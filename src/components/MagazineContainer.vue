<style lang="scss">

.cover{
  background-image: url("/img/pages/g-0.jpg");
  background-position: center;
  background-repeat: no-repeat;
  background-size: cover;
  position: relative;
}
.magazine-container#blur.active{
  filter: blur(15px);
  // pointer-events: none;
  user-select: none;
}
.magazine-container.active{
    top: 50%;
    visibility: visible;
    opacity: 1;
    transform: 0.5s;
}

.magazine-container {
  display: flex;
  flex: 1;
  flex-flow: column;

  .header {
    display: flex;
    padding: 15px;
    transition: 500ms;
    position: relative;

    .menu-container,
    .menu-toggle {
      display: none;
    }

    @media (min-width: $breakpoint-sm) and (max-width: 480px) {
      .menu-toggle {
        display: block;
        background-color: #ffffff;
        bottom: 0;
        color: $primary-color;
        height: 40px;
        position: absolute;
        margin-top: auto;
        margin-bottom: auto;
        top: 0;
        width: 40px;
      }

      .menu-container {
        display: flex;
        flex-flow: column;
        position: absolute;
        border-radius: 10px;
        width: auto;
        height: auto;
        z-index: 9998;
        top: 75px;
        visibility: hidden;
        opacity: 0;
        transition: 250ms;

        &.active {
          visibility: visible;
          opacity: 1;
        }

        .menu-btn {
          margin-top: 5px;
        }

        .language-list {
          display: flex;
          flex-flow: column;
          max-height: 10px;
          transition: 250ms;

          &.active {
            max-height: 145px;
          }

          .language {
            background-color: #ffffff;
            border: none;
            // font-size: 25px;
            margin-top: 10px;
            margin-left: auto;
            margin-right: auto;
            padding: 0px;
            border-radius: 50px;
            width: 33px;
            height: 33px;

            svg {
              display: block;
              fill: $primary-color-v;
              margin: auto;
            }

            &:hover {
              background-color: rgba($color: $secondary-color-v, $alpha: 0.7);
            }

            &:active {
              background-color: rgba($color: $secondary-color-v, $alpha: 0.7);
            }

            &.active {
              background-color: rgba($color: $secondary-color-v, $alpha: 0.7);
            }
          }
        }
      }
    }

    .search-group {
      margin: 0 auto;
      width: auto;
      position: relative;

      .search {
        background-color: $primary-color;
        border: 1px solid #ffffff;
        border-radius: 10px;
        color: #ffffff;
        display: block;
        font-weight: 400;
        padding: 20px;
        transition: 500ms;
        width: 200px;

        &::-webkit-input-placeholder {
          color: #ffffff;
        }

        &:hover::-webkit-input-placeholder,
        &:focus::-webkit-input-placeholder {
          color: $primary-color;
        }

        &:hover {
          background-color: #ffffff;
          color: $primary-color;
        }
      }
    }

    &.searchFocus {
      background-color: $primary-color;

      .menu-toggle {
        display: none;
      }

      .search {
        width: 300px;
        background-color: #ffffff;
        color: $primary-color;

        @media (min-width: $breakpoint-sm) and (max-width: 480px) {
          width: 200px;
        }

        &::-webkit-input-placeholder {
          color: $primary-color;
        }
      }

      .search-close {
        opacity: 1;
      }
    }

    .search-close {
      position: absolute;
      right: -50px;
      top: 0;
      bottom: 0;
      margin-top: auto;
      margin-bottom: auto;
      background-color: #ffffff;
      color: $primary-color;
      width: 40px;
      height: 40px;
      opacity: 0;
    }
  }

  .search-wrapper {
    background-color: $primary-color;
    color: #ffffff;
    height: 100%;
    opacity: 0;
    position: absolute;
    transition: 500ms;
    width: 100%;

    &.searchFocus {
      opacity: 1;
      z-index: 99999;
    }

    .search-container {
      background-color: #ffffff;
      border-radius: 10px;
      display: flex;
      flex-flow: column;
      margin-left: auto;
      margin-right: auto;
      padding: 20px;
      width: 30%;
      max-height: 100%;
      transition: max-height 500ms;

      @media (min-width: $breakpoint-lg) and (max-width: ($breakpoint-xl - 1px)) {
        width: 50%;
      }

      @media (min-width: $breakpoint-md) and (max-width: ($breakpoint-lg - 1px)) {
        width: 80%;
      }

      @media (min-width: 481px) and (max-width: ($breakpoint-md - 1px)) {
        width: 80%;
      }

      @media (min-width: $breakpoint-sm) and (max-width: 480px) {
        width: 90%;
      }

      .search-result-title {
        color: $primary-color;
        border-bottom: 1px solid #eeeeee;
        padding-bottom: 10px;
      }

      .list-group {
        flex: 1;
        list-style-type: none;
        margin-top: 15px;
        max-height: 100%;
        overflow-y: auto;
        scroll-behavior: smooth;

        &::-webkit-scrollbar {
          width: 0px;
        }

        .list-group-item {
          border-bottom: 1px solid #eeeeee;
          border-radius: 10px;
          margin-bottom: 10px;
          width: 100%;
          padding: 10px;
          transition: 500ms;
          cursor: pointer;
          background-color: #f5f5f5;

          &:hover {
            background-color: $secondary-color-v;

            a {
              color: #ffffff;
            }
          }

          a {
            color: $primary-color;
            text-decoration: none;
          }
        }
      }
    }
  }

  .magazine-wrapper {
    align-items: center;
    display: flex;
    position: relative;
    flex: 1;
    overflow: hidden;
    position: relative;

    .zoom-wrapper {
      overflow: hidden;
      position: relative;
      height: 100%;
      width: 100%;

      .zoom {
        display: flex;
        min-height: 100%;
        height: 100%;

        .magazine {
          margin: auto;

          @media (min-width: $breakpoint-xl) {
            height: 693.11px;
            width: 980px;
          }

          @media (min-width: $breakpoint-lg) and (max-width: ($breakpoint-xl - 1px)) {
            height: 495.08px;
            width: 700px;
          }

          @media (min-width: 481px) and (max-width: ($breakpoint-lg - 1px)) {
            height: 600px;
            width: 420px;
          }

          @media (min-width: $breakpoint-sm) and (max-width: 480px) {
            height: 466.79px;
            width: 330px;
          }

          .p1 {
            .cover {
              height: 100%;
              visibility: hidden;

              video {
                display: none;
                position: fixed;
                top: 50%;
                left: 50%;
                min-width: 100%;
                min-height: 100%;
                width: auto;
                height: auto;
                z-index: -100;
                -webkit-transform: translateX(-50%) translateY(-50%);
                transform: translateX(-50%) translateY(-50%);
              }
            }
          }

          .page {
            background-color: #ffffff;
            font-size: 0.8rem;

            .highlight {
              background-color: #fff76a;
              color: #1f354c;
            }
          }
        }
      }
    }
  }

  .footer {
    display: flex;
    justify-content: center;
    padding: 15px;
    position: relative;
    bottom: 40px;
    transition: 500ms;

    @media (min-width:1440px) {
      bottom: 70px;
    }

    &.searchFocus {
      background-color: $primary-color;

      .btn-comment {
        opacity: 0;
        top: 0px;
      }
    }

    .btn {
      @media (min-width: $breakpoint-sm) and (max-width: 480px) {
        opacity: 1;
      }

      opacity: 0;
      height: 40px;
      width: 40px;
    }

    .btn-comment {
      background-color: #ffffff;
      color: $primary-color-v;
      border-radius: 50px;
      height: 40px;
      position: absolute;
      margin-left: 0;
      margin-right: 0;
      left: 15px;
      width: 40px;

      &.active {
        color: $secondary-color-v;
        transform: scale(1.1);
      }
    }

    .comments-wrapper {
      background-color: rgba($color: $primary-color, $alpha: 1);
      color: $primary-color;
      border-radius: 10px;
      bottom: 70px;
      display: flex;
      flex-flow: column;
      height: 0px;
      left: 10px;
      padding: 10px;
      position: absolute;
      width: 400px;
      transition: opacity 500ms, height 250ms;
      -webkit-box-shadow: -8px 8px 20px 0px rgba(0, 0, 0, 0.3);
      -moz-box-shadow: -8px 8px 20px 0px rgba(0, 0, 0, 0.3);
      box-shadow: -8px 8px 20px 0px rgba(0, 0, 0, 0.3);
      visibility: hidden;
      z-index: 9999;
      opacity: 0;

      @media (min-width: $breakpoint-sm) and (max-width: 480px) {
        width: calc(100% - 20px);
      }

      &.isActive {
        visibility: visible;
        height: 500px;
        opacity: 1;

        @media (min-width: $breakpoint-lg) and (max-width: ($breakpoint-xl - 1px)) {
          height: calc(100vh - 80px);
        }

        @media (min-width: 481px) and (max-width: ($breakpoint-lg - 1px)) {
          height: calc(100vh - 80px);
        }

        @media (min-width: $breakpoint-sm) and (max-width: 480px) {
          height: calc(100vh - 80px);
          width: calc(100% - 20px);
        }
      }

      .comments {
        flex: 1;
        display: flex;
        flex-flow: column;
        overflow: hidden;

        .comments-title {
          border-bottom: 1px solid $primary-color-v;
          padding: 10px;
          display: flex;

          .title {
            align-self: center;
            color: #ffffff;
            font-weight: 900;
          }

          button {
            margin-left: auto;
            width: 40px;

            &:hover {
              transform: scale(1);
            }

            &:active {
              transform: scale(0.9);
            }
          }
        }

        .comments-card {
          display: flex;
          flex: 1;
          flex-flow: column;
          font-size: 0.8rem;
          overflow: hidden;
          padding: 10px;

          .comments-list {
            flex: 1;
            list-style: none;
            max-height: 0;
            opacity: 0;
            overflow-y: auto;
            scroll-behavior: smooth;
            transition: 500ms;
            visibility: hidden;

            &.active {
              max-height: none;
              opacity: 1;
              visibility: visible;
            }

            &::-webkit-scrollbar {
              width: 5px;
            }

            &::-webkit-scrollbar-track {
              background: #eeeeee;
              border-radius: 50px;
            }

            &::-webkit-scrollbar-thumb {
              background: $secondary-color-v;
              border-radius: 10px;
            }

            li:last-child .comment {
              border-bottom: none;
            }

            .comment {
              border-bottom: 1px solid $primary-color-v;
              color: #ffffff;
              padding: 10px;

              .title {
                display: flex;

                .user {
                  background-color: $secondary-color-v;
                  border-radius: 50px;
                  display: flex;
                  color: #ffffff;
                  height: 50px;
                  width: 50px;
                  align-items: center;
                  justify-content: center;
                }

                .details {
                  display: flex;
                  flex: 1;
                  flex-flow: column;
                  justify-content: center;
                  line-height: 20px;
                  margin-left: 10px;
                }
              }

              .text {
                margin-top: 10px;
                line-height: 20px;
              }
            }
          }

          .comment-input {
            color: #ffffff;
            flex: 1;
            max-height: 0;
            opacity: 0;
            position: relative;
            transition: 500ms;
            visibility: hidden;

            &.active {
              max-height: none;
              visibility: visible;
              opacity: 1;
            }

            .input-group {
              display: flex;
              flex-flow: column;
              margin-bottom: 15px;

              label {
                margin-bottom: 5px;
              }

              input,
              textarea {
                border: 2px solid #dddddd;
                border-radius: 5px;
                padding: 8px;
                resize: none;
              }

              &.invalid {
                label {
                  color: $secondary-color-v;
                }

                input,
                textarea {
                  border: 2px solid $secondary-color-v;
                }
              }
            }

            button {
              height: 40px;
              // width: 40px;
              bottom: 10px;
            }
          }
        }
      }
    }

    &:not(.searchFocus) .tools-container:hover .btn {
      opacity: 1;
    }
  }
}

#image-modal {
  background-color: rgba($color: $primary-color, $alpha: 0.9);
  position: absolute;
  left: 0;
  top: 0;
  right: 0;
  bottom: 0;
  width: 100%;
  height: 100%;

  z-index: -9999;
  visibility: hidden;
  opacity: 0;
  transition: 500ms;

   //showImage zoom image
  &.active {
    z-index: 9999;
    visibility: visible;
    opacity: 1;
  }

  .image-container {
    position: relative;
    width: 100%;
    height: 100%;

    img {
      position: absolute;
      top: 50%;
      left: 50%;
      transform: translate(-50%, -50%);
      max-height: 80%;
      max-width: 90%;
    }
  }
}



#table_of_contents {
  background-color: $primary-color;
  z-index: -9999;

  display: flex;
  flex-flow: column;

  position: absolute;
  top: 0;
  bottom: 0;
  left: -100vh;
  // right: 0;

  height: 100%;
  width: 100%;

  visibility: hidden;
  opacity: 0;

  transition: 500ms;

  &.active {
    z-index: 9999;

    visibility: visible;
    opacity: 1;

    left: 0;
  }

  .menu-container {
    padding: 20px;
    color: #ffffff;

    display: flex;

    .title {
      margin-top: auto;
      margin-bottom: auto;
    }

    .close {
      height: 40px;
      width: 40px;

      margin-left: auto;
    }
  }

  ul {
    list-style-type: none;
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
      border-radius: 10px;
    }

    li {
      background-color: $primary-color-v;
      border-radius: 10px;
      color: #ffffff;
      font-size: 0.8rem;
      margin-left: 15px;
      margin-right: 15px;
      transition: 500ms;

      div {
        padding: 20px;
        margin-bottom: 10px;
      }
    }
  }
}
</style>

<template>
  <div class="magazine-container">
    <div class="header" :class="{ searchFocus: isSearchFocus }">
      <Button
        class="menu-toggle"
        v-on:click.native="
          menu.toggled = !menu.toggled;
          language.toggled = false;
        "
      >
        <i class="fas fa-bars"></i>
      </Button>
      <div class="search-group">
        <input
          :id="search"
          class="search"
          type="search"
          :placeholder="$t('search') + '...'"
          ref="search"
          v-model="searchField"
          @focus="searchFocus(true)"
          @input="search"
          @keypress.enter="searchTurnPage"
        />
        <Button class="search-close" v-on:click.native="searchFocus(false)">
          <i class="fas fa-times"></i>
        </Button>
      </div>
      <div class="menu-container" :class="{ active: menu.toggled }">
        <Button class="menu-btn" v-on:click.native="highlight">
          <i class="fas fa-highlighter fa-lg"></i>
        </Button>
        <Button
          class="menu-btn"
          v-on:click.native="language.toggled = !language.toggled"
        >
          <i class="fas fa-language fa-lg"></i>
        </Button>
        <div class="language-list" :class="{ active: language.toggled }">
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
        <Button
          class="menu-btn menu-content-toggle-btn"
          v-on:click.native="
            tableOfContent.active = !tableOfContent.active;
            menu.toggled = false;
          "
        >
          <i class="fas fa-list-ol fa-lg"></i>
        </Button>
        <Button
          class="menu-btn menu-content-toggle-btn"
          v-on:click.native="
            bookmark.active = !bookmark.active;
            menu.toggled = false;
          "
        >
          <i class="far fa-bookmark"></i>
        </Button>
        <Button class="menu-btn" v-on:click.native="getSelText">
          <i class="fas fa-sticky-note"></i>
        </Button>
        <Button class="menu-btn" v-on:click.native="speech">
          <i class="fas fa-volume-up"></i>
        </Button>  
        <Button class="menu-btn" v-on:click.native="star">
        <i class="far fa-star"></i>
      </Button>     
      <Button class="menu-btn" v-on:click.native="searchSpeak">
        <i class="fas fa-microphone"></i>
      </Button>     
      </div>
    </div>

    <div class="magazine-wrapper">
      <div class="search-wrapper" :class="{ searchFocus: isSearchFocus }">
        <div class="search-container">
          <div class="search-result-title">
            <h3>{{ $t("search_result") }}</h3>
          </div>

          <ul class="list-group">
            <li
              class="list-group-item"
              v-for="search in searchResult"
              v-bind:key="search.id"
              v-on:click="searchPage(search.page)"
            >
              <a href="#" v-html="search.text"></a>
            </li>
          </ul>
        </div>
      </div>

      <div class="zoom-wrapper">
        <div class="zoom">
          <div
            id="magazine"
            class="magazine"
          >
            <div class="cover">
            </div>
            <Page1 />
            <Page2 />
            <Page3 />
            <Page4 />
            <Page5 />
            <Page6 />
            <Page7 />
            <Page8 />
            <Page9 />
            <Page10 />
            <Page11 />
            <Page12 />
            <Page13 />
            <Page14 />
            <Page15 />
          </div>
        </div>
      </div>

      <Sidebar>
        
        <template v-slot:table_of_contents>
          <li>
            <div
              v-on:click="
                turnPage(2);
                tableOfContent.active = false;
              "
            >
              {{ $t("table_of_contents_items.title1") }}
            </div>
          </li>
          <li>
            <div
              v-on:click="
                turnPage(4);
                tableOfContent.active = false;
              "
            >
              {{ $t("table_of_contents_items.title2") }}
            </div>
          </li>
          <li>
            <div
              v-on:click="
                turnPage(6);
                tableOfContent.active = false;
              "
            >
              {{ $t("table_of_contents_items.title3") }}
            </div>
          </li>
          <li>
            <div
              v-on:click="
                turnPage(8);
                tableOfContent.active = false;
              "
            >
              {{ $t("table_of_contents_items.title4") }}
            </div>
          </li>
          <li>
            <div
              v-on:click="
                turnPage(10);
                tableOfContent.active = false;
              "
            >
              {{ $t("table_of_contents_items.title5") }}
            </div>
          </li>
          <li>
            <div
              v-on:click="
                turnPage(12);
                tableOfContent.active = false;
              "
            >
              {{ $t("table_of_contents_items.title6") }}
            </div>
          </li>
          <li>
            <div
              v-on:click="
                turnPage(13);
                tableOfContent.active = false;
              "
            >
              {{ $t("table_of_contents_items.title7") }}
            </div>
          </li>
          <li>
            <div
              v-on:click="
                turnPage(14);
                tableOfContent.active = false;
              "
            >
              {{ $t("table_of_contents_items.title8") }}
            </div>
          </li>
          <li>
            <div
              v-on:click="
                turnPage(16);
                tableOfContent.active = false;
              "
            >
              {{ $t("table_of_contents_items.title9") }}
            </div>
          </li>
          
        </template>
        <template v-slot:favorit >
          <li v-for="(star,index) of stars" v-bind:key="star">
            <div
              v-on:click="
                turnPage(star);
                bookmark.active = false;
              "
            >
              {{ star == 1 ? "Genzius Berbagi Informasi" : ""}} {{ star == 2 ? "Maspion Pelopori Kebangkitan Ekonomi Di Masa Pandemi" : ""}} {{ star == 3 ? "Maspion Pelopori Kebangkitan Ekonomi Di Masa Pandemi" : ""}} {{ star == 4 ? "Maspion Pelopori Kebangkitan Ekonomi Di Masa Pandemi" : ""}} {{ star == 5 ? "puki" : ""}} {{ star == 6 ? "Salam" : ""}} {{ star == 7 ? "Salam" : ""}} {{ star == 8 ? "Salam" : ""}} {{ star == 9 ? "Salam" : ""}} {{ star == 10 ? "Salam" : ""}} {{ star == 11 ? "Salam" : ""}} {{ star == 12 ? "Salam" : ""}} {{ star == 13 ? "Salam" : ""}} {{ star == 14 ? "Salam" : ""}} {{ star == 15 ? "Salam" : ""}} {{ star == 16 ? "Salam" : ""}}
            </div> <button v-on:click="hpsf(index)" class="ok"><i class="fas fa-trash"></i></button> 
          </li>
        </template>
      </Sidebar>
    </div>

    <div class="footer" :class="{ searchFocus: isSearchFocus }">
      <div class="tools-container">
        <Button class="btn" v-on:click.native="doublePreviousPage">
          <i class="fas fa-angle-double-left fa-lg"></i>
        </Button>
        <Button class="btn" v-on:click.native="previousPage">
          <i class="fas fa-angle-left fa-lg"></i>
        </Button>
        <Button class="btn" v-on:click.native="nextPage">
          <i class="fas fa-angle-right fa-lg"></i>
        </Button>
        <Button class="btn" v-on:click.native="doubleNextPage">
          <i class="fas fa-angle-double-right fa-lg"></i>
        </Button>
      </div>
      <Button
        class="btn-comment"
        :class="{ active: toggleCommentStatus }"
        v-on:click.native="toggleComment"
      >
        <i class="fas fa-sticky-note"></i>
      </Button>

      <div
        class="comments-wrapper"
        :class="{ isActive: toggleCommentStatus, isInput: inputComment }"
      >
        <div class="comments">
          <div class="comments-title">
            <h4 class="title">{{ $t("comment") }}</h4>
            <Button v-on:click.native="toggleCommentInput">
              <i
                class="fas"
                :class="{
                  'fa-plus': !inputComment,
                  'fa-arrow-left': inputComment,
                }"
              ></i>
            </Button>
          </div>
          <div class="comments-card">
            <div class="comment-input" :class="{ active: inputComment }">
              <div class="input-group" :class="{ invalid: !commentText.valid }">
                <label for="text">{{ $t("comment") }}</label>
                <textarea
                  id="tambah"
                  rows="5"
                ></textarea>
              </div>
              <button v-on:click="tambah">{{ $t("comment_post") }}</button>
            </div>
            <ul class="comments-list" :class="{ active: !inputComment }">
              <li v-for="(note,index) of selects" :key="note.id" >
                <div class="comment">{{ note }}</div>
                <button v-on:click="hps(index)"><i class="fas fa-trash"></i></button>
              </li>
            </ul>
          </div>
        </div>
      </div>
    </div>

    <div id="image-modal" :class="{ active: image.active }">
      <div class="image-container" v-on:click="image.active = !image.active">
        <img src="" alt="" srcset="" />
      </div>
    </div>

    <div id="table_of_contents" :class="{ active: tableOfContent.active }">
      <div class="menu-container">
        <span class="title">{{ $t("table_of_contents") }}</span>
        <Button class="close" v-on:click.native="tableOfContent.active = false"
          ><i class="fas fa-times"></i
        ></Button>
      </div>
      <ul>
        <li>
          <div
            v-on:click="
              turnPage(2);
              tableOfContent.active = false;
            "
          >
            {{ $t("table_of_contents_items.title1") }}
          </div>
        </li>
        <li>
          <div
            v-on:click="
              turnPage(4);
              tableOfContent.active = false;
            "
          >
            {{ $t("table_of_contents_items.title2") }}
          </div>
        </li>
        <li>
          <div
            v-on:click="
              turnPage(6);
              tableOfContent.active = false;
            "
          >
            {{ $t("table_of_contents_items.title3") }}
          </div>
        </li>
        <li>
          <div
            v-on:click="
              turnPage(8);
              tableOfContent.active = false;
            "
          >
            {{ $t("table_of_contents_items.title4") }}
          </div>
        </li>
        <li>
          <div
            v-on:click="
              turnPage(10);
              tableOfContent.active = false;
            "
          >
            {{ $t("table_of_contents_items.title5") }}
          </div>
        </li>
        <li>
          <div
            v-on:click="
              turnPage(12);
              tableOfContent.active = false;
            "
          >
            {{ $t("table_of_contents_items.title6") }}
          </div>
        </li>
        <li>
          <div
            v-on:click="
              turnPage(13);
              tableOfContent.active = false;
            "
          >
            {{ $t("table_of_contents_items.title7") }}
          </div>
        </li>
        <li>
          <div
            v-on:click="
              turnPage(14);
              tableOfContent.active = false;
            "
          >
            {{ $t("table_of_contents_items.title8") }}
          </div>
        </li>
        <li>
          <div
            v-on:click="
              turnPage(16);
              tableOfContent.active = false;
            "
          >
            {{ $t("table_of_contents_items.title9") }}
          </div>
        </li>
      </ul>
    </div>
    
    <div id="table_of_contents" :class="{ active: bookmark.active }">
      <div class="menu-container">
        <span class="title">FAVORIT</span>
        <Button class="close" v-on:click.native="bookmark.active = false"
          ><i class="fas fa-times"></i
        ></Button>
      </div>
      <ul>
        <li v-for="(star,index) of stars" v-bind:key="star">
          <div
            v-on:click="
              turnPage(star);
              bookmark.active = false;
            "
          >
          {{ star == 1 ? "Genzius Berbagi Informasi" : ""}} {{ star == 2 ? "Maspion Pelopori Kebangkitan Ekonomi Di Masa Pandemi" : ""}} {{ star == 3 ? "Maspion Pelopori Kebangkitan Ekonomi Di Masa Pandemi" : ""}} {{ star == 4 ? "Maspion Pelopori Kebangkitan Ekonomi Di Masa Pandemi" : ""}} {{ star == 5 ? "puki" : ""}} {{ star == 6 ? "Salam" : ""}} {{ star == 7 ? "Salam" : ""}} {{ star == 8 ? "Salam" : ""}} {{ star == 9 ? "Salam" : ""}} {{ star == 10 ? "Salam" : ""}} {{ star == 11 ? "Salam" : ""}} {{ star == 12 ? "Salam" : ""}} {{ star == 13 ? "Salam" : ""}} {{ star == 14 ? "Salam" : ""}} {{ star == 15 ? "Salam" : ""}} {{ star == 16 ? "Salam" : ""}}
            </div> <button v-on:click="hpsf(index)" class="book"><i class="fas fa-trash"></i></button> 
        </li>
      </ul>
    </div>
  </div>
</template>

<script>
import Sidebar from "@/components/Sidebar.vue";
import Button from "@/components/Button.vue";
import Page1 from "@/components/pages/Page1.vue";
import Page2 from "@/components/pages/Page2.vue";
import Page3 from "@/components/pages/Page3.vue";
import Page4 from "@/components/pages/Page4.vue";
import Page5 from "@/components/pages/Page5.vue";
import Page6 from "@/components/pages/Page6.vue";
import Page7 from "@/components/pages/Page7.vue";
import Page8 from "@/components/pages/Page8.vue";
import Page9 from "@/components/pages/Page9.vue";
import Page10 from "@/components/pages/Page10.vue";
import Page11 from "@/components/pages/Page11.vue";
import Page12 from "@/components/pages/Page12.vue";
import Page13 from "@/components/pages/Page13.vue";
import Page14 from "@/components/pages/Page14.vue";
import Page15 from "@/components/pages/Page15.vue";
import jQuery from "jquery";

window.jQuery = jQuery;
require("@/assets/turn.min.js");

export default {
  name: "MagazineWrapper",
  components: {
    Sidebar,
    Button,
    Page1,
    Page2,
    Page3,
    Page4,
    Page5,
    Page6,
    Page7,
    Page8,
    Page9,
    Page10,
    Page11,
    Page12,
    Page13,
    Page14,
    Page15,
  },
  data() {
    return {
      selects: [],
      isSearchFocus: false,
      searchField: "",
      searchResult: [],
      inputComment: false,
      comments: [],
      commentName: {
        data: "",
        valid: true,
      },
      commentEmail: {
        data: "",
        valid: true,
      },
      commentText: {
        data: "",
        valid: true,
      },
      toggleCommentStatus: false,
      menu: {
        toggled: false,
      },
      language: {
        toggled: false,
        data: "id",
      },
      image: {
        active: false,
      },
      tableOfContent: {
        active: false,
      },
      bookmark: {
        active: false
      },
      synth: window.speechSynthesis,
      stars:[],
      lastSeen : "1",
      lang_: "en-EN",
      isSpeak: false
    };
  },
  mounted() {
    const magazine = window.jQuery(".magazine");
    const mediaQuery = window.matchMedia("(max-width: 1024px)");

    if (mediaQuery.matches) {
      magazine.turn({ display: "single" });
    } else {
      magazine.turn({ display: "double" });
    }
    
    if (localStorage.selects) {
      this.selects = JSON.parse(localStorage.selects);
    }

    if (localStorage.stars) {
      this.stars = JSON.parse(localStorage.stars);
    }
    
    if (localStorage.lastSeen) {
      this.lastSeen = localStorage.lastSeen;
    }
    
    magazine.bind('turned', (event, page) => {
      console.log('Page: ', page)
      this.lastSeen =  window.jQuery(".magazine").turn("page");
      this.localStorage();
    })

    window.onload = this.onload()
  },
  methods: {
    // DARI HIL
    tambah: function () {
      let text = document.getElementById("tambah").value;
      if (text != "") {
        this.selects.push(text);
      } else {
        alert("isi dulu");
      }
      this.localStorage();
      document.getElementById("tambah").value = "";
    },
    hps(id) {
      this.selects.splice(id, 1)
      this.localStorage()
    },
    hpsf(id) {
      this.stars.splice(id, 1)
      this.localStorage()
    },
    speech: function(){
      this.isSpeak = !this.isSpeak;
      var txt = [];
      if (window.getSelection) {
        txt = window.getSelection();
      }
      let utterance = new SpeechSynthesisUtterance(""+txt);   
      utterance.lang = 'id-ID'
      utterance.rate = 1
      if ("" + txt != "") {
        if(this.isSpeak == true){
          this.synth.speak(utterance);
        } 
        else {
          this.synth.cancel();
        }
      } else {
          alert("silahkan pilih text terlebih dahulu");
      }
    },
    getSelText: function () {
      var txt = [];
      if (window.getSelection) {
        txt = window.getSelection();
      }
      if ("" + txt != "") {
        this.selects.push("" + txt);
      } else {
        alert("silahkan pilih text terlebih dahulu");
      }
      this.localStorage();
    },
    star: function(){
      let text = window.jQuery(".magazine").turn("page");
      if (this.stars.includes(text)) {
        console.log("sudah ada")
      } else {
        this.stars.push(text)
        this.localStorage()
        console.log(this.stars)
      }
      
    },
    searchSpeak: function (){
    window.SpeechRecognition =
    window.SpeechRecognition || 
    window.webkitSpeechRecognition;
    const recognition = new window.SpeechRecognition();
    recognition.lang = this.lang_;
    recognition.continuous = false;
    recognition.interimResults = true;
    recognition.maxAlternatives = 1;
    // recognition.interimResults = true;
    recognition.addEventListener("result", event => {      
      var pages = event.results[0][0].transcript;
      var page = parseInt(pages)
      this.turnPage(page+1);
    });
    // end of transcription
    recognition.addEventListener("end", () => {
      recognition.stop();
    });
     recognition.start();
    },
    localStorage: function () {
      localStorage.setItem("selects", JSON.stringify(this.selects));
      localStorage.setItem("stars", JSON.stringify(this.stars));
      localStorage.setItem("lastSeen", JSON.stringify(this.lastSeen));
    },
    onload(){
      this.turnPage(this.lastSeen)
    },
    // DARI HIL

    turnPage(page) {
      const magazine = window.jQuery(".magazine");
      if (magazine.turn("hasPage", page)) magazine.turn("page", page);
    },
    nextPage() {
      const magazine = window.jQuery(".magazine");
      magazine.turn("next");
    },
    previousPage() {
      const magazine = window.jQuery(".magazine");
      magazine.turn("previous");
    },
    doubleNextPage() {
      const magazine = window.jQuery(".magazine");
      let page = magazine.turn("page") + 2;
      console.log(page);
      if (magazine.turn("hasPage", page) && page > 0)
        magazine.turn("page", page);
      else magazine.turn("page", 33);
    },
    doublePreviousPage() {
      const magazine = window.jQuery(".magazine");
      let page = magazine.turn("page") - 2;
      console.log(page);
      if (magazine.turn("hasPage", page) && page > 0)
        magazine.turn("page", page);
      else magazine.turn("page", 1);
    },
    highlight() {
      const range = window.getSelection().getRangeAt(0),
      span = document.createElement("mark");
      span.appendChild(range.extractContents());
      range.insertNode(span);
    },
    searchFocus(focus) {
      this.isSearchFocus = focus;
      if (!focus) this.searchField = "";
      this.menu.toggled = false;
      this.language.toggled = false;
    },
    search() {
      let searched = this.searchField;
      let id = 1;

      if (searched !== "") {
        let text = document
          .getElementById("magazine")
          .getElementsByTagName("span");

        this.searchResult = [];

        window.jQuery.each(text, (_, val) => {
          const value = window.jQuery(val).text();
          let re = new RegExp(searched, "i");

          if (value.toLowerCase().indexOf(searched) !== -1) {
            // let parent = window.jQuery(val).parent().parent().parent().parent();
            let parent = window.jQuery(val).closest(".page");
            const page = window
              .jQuery(parent)
              .attr("class")
              .match(/p\d+/)[0]
              .substring(1);
            let text = value.replace(re, `<mark>${searched}</mark>`);

            this.searchResult.push({
              id: id,
              page: page,
              text: text,
            });
            id++;
          } else if (value.indexOf(searched) !== -1) {
            // let parent = window.jQuery(val).parent().parent().parent().parent();
            let parent = window.jQuery(val).closest(".page");
            const page = window
              .jQuery(parent)
              .attr("class")
              .match(/p\d+/)[0]
              .substring(1);
            let text = value.replace(re, `<mark>${searched}</mark>`);

            this.searchResult.push({
              id: id,
              page: page,
              text: text,
            });

            id++;
          }
        });
      } else {
        this.searchResult = [];
      }
    },
    searchPage(page) {
      this.isSearchFocus = false;
      const magazine = window.jQuery(".magazine");
      setTimeout(() => {
        magazine.turn("page", page);
      }, 200);
    },
    searchTurnPage() {
      if (this.searchField !== "") {
        const magazine = window.jQuery(".magazine");
        let page = parseInt(this.searchField) + 1;
        if (magazine.turn("hasPage", page)) {
          magazine.turn("page", page);
          this.isSearchFocus = false;
          this.$refs.search.blur();
        }
      }
    },
    toggleComment() {
      this.toggleCommentStatus = !this.toggleCommentStatus;
    },
    toggleCommentInput() {
      this.inputComment = !this.inputComment;
    },
    changeLanguage(lang) {
      this.$i18n.locale = lang;
      this.language.data = lang;
    },
    showImage(url) {
      this.image.active = true;
      document
        .getElementById("image-modal")
        .getElementsByTagName("img")[0].src = url;
    },
  },
};
</script>