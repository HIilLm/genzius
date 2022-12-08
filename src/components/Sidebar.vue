<style lang="scss" scoped>
.sidebar {
  background-color: rgba($color: $primary-color, $alpha: 1);
  -webkit-box-shadow: 8px 8px 20px 0px rgba(0, 0, 0, 0.3);
  -moz-box-shadow: 8px 8px 20px 0px rgba(0, 0, 0, 0.3);
  box-shadow: 8px 8px 20px 0px rgba(0, 0, 0, 0.3);
  border-radius: 15px 0 0 15px;
  display: flex;
  max-height: 100%;
  padding: 20px;
  position: absolute;
  transition: 300ms;
  width: 400px;
  right: -380px;

  @media (min-width: $breakpoint-sm) and (max-width: 480px) {
    display: none;
  }

  &:hover {
    right: -325px;
  }

  &.active {
    right: -325px;

    .menu-toggle-btn {
      color: $secondary-color-v;
      transform: scale(1.1);

      &:active {
        transform: scale(0.98);
      }
    }
  }

  &.contentActive:hover {
    right: 0px;

    .menu-content-toggle-btn {
      color: $secondary-color-v;
      transform: scale(1.1);
    }

    &:active {
      transform: scale(0.98);
    }
  }

  &.active.contentActive {
    right: 0px;

    .menu-toggle-btn,
    .menu-content-toggle-btn {
      color: $secondary-color-v;
      transform: scale(1.1);

      &:active {
        transform: scale(0.98);
      }
    }
  }

  .menu-container {
    border-right: 2px solid $primary-color-v;
    display: flex;
    flex-flow: column;
    padding-right: 10px;

    .menu-toggle-btn {
      height: 40px;
      width: 40px;
    }

    .menu-btn,
    .menu-content-toggle-btn {
      height: 40px;
      margin-top: 10px;
      width: 40px;
    }

    .language-list {
      background-color: $primary-color-v;
      border-radius: 10px;
      display: flex;
      flex-flow: column;
      margin-top: 10px;
      max-height: 46px;
      overflow: hidden;
      padding-top: 3px;
      padding-bottom: 7px;
      transition: max-height 500ms;

      &.active {
        max-height: 249px;

        .toggle {
          transform: scale(1.1);
          color: $secondary-color-v;
        }
      }

      .menu-btn {
        margin-top: 0;

        &.language {
          background-color: transparent;
          border: none;
          font-size: 25px;
          margin-top: 10px;
          margin-left: auto;
          margin-right: auto;
          padding: 0px;
          border-radius: 50px;
          width: 33px;
          height: 33px;

          svg {
            display: block;
            fill: #ffffff;
            margin: auto;
          }

          &:hover {
            transform: scale(1.2);
            background-color: rgba($color: $secondary-color-v, $alpha: 0.7);
          }

          &:active {
            transform: scale(0.98);
            background-color: rgba($color: $secondary-color-v, $alpha: 0.7);
          }

          &.active {
            transform: scale(1.2);
            background-color: rgba($color: $secondary-color-v, $alpha: 0.7);
          }
        }
      }
    }
  }

  .contents-container {
    display: flex;
    flex: 1;
    flex-flow: column;

    .title {
      color: #ffffff;
      padding-left: 15px;
      margin-bottom: 15px;
    }

    .list-group {
      flex: 1;
      overflow: auto;

      &::-webkit-scrollbar {
        width: 5px;
      }

      &::-webkit-scrollbar-track {
        background: #eeeeee;
        border-radius: 50px;
      }

      &::-webkit-scrollbar-thumb {
        background: $secondary-color-v;
        border-radius: 50px;
      }

      ul {
        list-style-type: none;

        li {
          background-color: $primary-color-v;
          border-radius: 10px;
          color: #ffffff;
          font-size: 0.8rem;
          margin-bottom: 15px;
          margin-left: 15px;
          margin-right: 15px;
          transition: 500ms;

          &:hover {
            background-color: rgba($color: $primary-color-v, $alpha: 0.5);
            transform: scale(1.05);
          }

          div {
            cursor: pointer;
            padding: 10px;
          }
        }
      }
    }
  }
}
</style>

<template>
  <div
    class="sidebar"
    v-bind:class="{ active: isActive , isMark, contentActive: isBook , isContentActive }"
  >
    <div class="menu-container">
      <Button class="menu-toggle-btn" v-on:click.native="toggle">
        <i class="fas fa-circle fa-lg"></i>
      </Button>
      <Button class="menu-btn" v-on:click.native="highlight">
        <i class="fas fa-highlighter fa-lg"></i>
      </Button>
      <div class="language-list" :class="{ active: language.active }">
        <Button
          class="menu-btn toggle"
          v-on:click.native="language.active = !language.active"
        >
          <i class="fas fa-language fa-lg"></i>
        </Button>
        <Button
          class="menu-btn language"
          :class="{ active: language.data == 'id' }"
          v-on:click.native="changeLanguage('id')"
        >
          <svg-icon icon="indonesia" />
        </Button>
        <Button
          class="menu-btn language"
          :class="{ active: language.data == 'en' }"
          v-on:click.native="changeLanguage('en')"
        >
          <svg-icon icon="united-kingdom" />
        </Button>
        <Button
          class="menu-btn language"
          :class="{ active: language.data == 'sby' }"
          v-on:click.native="changeLanguage('sby')"
        >
          <svg-icon icon="surabaya" />
        </Button>
      </div>
      <Button class="menu-content-toggle-btn" v-on:click.native="toggleContent(1)">
        <i class="fas fa-list-ol fa-lg"></i>
      </Button>
      <Button class="menu-content-toggle-btn" v-on:click.native="mark">
        <i class="fas fa-list-ol fa-lg"></i>
      </Button>
      <Button class="menu-btn" v-on:click.native="getSelText">
        <i class="fas fa-sticky-note"></i>
      </Button>
      <Button class="menu-btn" v-on:click.native="speech">
        <i class="fas fa-volume-up"></i>
      </Button>     
      <Button class="menu-btn" v-on:click.native="toggleContent(2)">
        <i class="far fa-bookmark"></i>
      </Button>     
      <Button class="menu-btn" v-on:click.native="star">
        <i class="far fa-star"></i>
      </Button>     
    </div>
    <div class="contents-container">
      <div class="title">{{ $t("table_of_contents") }}</div>
      <div class="list-group">
        <ul>
          <slot name="table_of_contents"></slot>
        </ul>
      </div>
    </div>
    <div class="contents-container">
      <div class="title">favorit</div>
      <div class="list-group">
        <ul>
          <slot name="favorit"></slot>
        </ul>
      </div>
    </div>
  </div>
</template>

<script>
import Button from "@/components/Button.vue";
export default {
  name: "Sidebar",
  components: {
    Button,
  },
  data() {
    return {
      hilang: true,
      isActive: false,
      isContentActive: false,
      isMark: false,
      isBook: false,
      language: {
        active: false,
        data: "id",
      },
    };
  },
  methods: {
    toggle(param) {
      if(param === 1){
        console.log("halo");
      }
      if(param === 2){
        console.log("merindu")
      }
      this.isActive = !this.isActive;
    },
    getSelText() {
      this.$parent.getSelText();
    },
    speech() {
      this.$parent.speech();
    },
    highlight() {
      this.$parent.highlight();
    },
    star(){
      this.$parent.star();
    },
    // zoomIn() {
    //   this.$parent.zoomIn();
    // },
    // zoomOut() {
    //   this.$parent.zoomOut();
    // },
    toggleContent() {
      this.isContentActive = !this.isContentActive;
    },
    mark() {
      this.isBook = !this.isBook;
    },
    changeLanguage(lang) {
      this.$i18n.locale = lang;
      this.language.data = lang;
    },
  },
};
</script>