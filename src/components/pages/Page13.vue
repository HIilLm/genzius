<style lang="scss">
.p14 {
  background-image: url("/img/pages/g-13.jpg");
  background-position: center;
  background-repeat: no-repeat;
  background-size: cover;
  position: relative;

  .content1 {
    color: #ffffff;
    position: absolute;
    top: 340px;
    left: 92px;
    width: 150px;

    .title {
      font-size: 2rem;
      line-height: 30px;

      @media (min-width: $breakpoint-sm) and (max-width: ($breakpoint-xl - 1px)) {
        font-size: 33px;
        line-height: 25px;
        width: 500px;
      }

      span {
        font-weight: 700;
      }
    }

    .subtitle {
      font-size: 1rem;

      @media (min-width: $breakpoint-sm) and (max-width: ($breakpoint-xl - 1px)) {
        font-size: 0.8rem;
        line-height: 15px;
      }
    }
  }
  .content {
    color: black;
    position: absolute;
    top: 15px;
    left: 20px;
    width: 150px;

    .title {
      font-size: 2rem;
      line-height: 30px;

      @media (min-width: $breakpoint-sm) and (max-width: ($breakpoint-xl - 1px)) {
        font-size: 35px;
        line-height: 40px;
        width: 20px;
      }

      span {
        font-weight: 700;
      }
    }

    .subtitle {
      font-size: 1rem;

      @media (min-width: $breakpoint-sm) and (max-width: ($breakpoint-xl - 1px)) {
        font-size: 0.8rem;
        line-height: 15px;
      }
    }
  }
  .content2 {
    position: absolute;
    text-align: justify;
    top: 385px;
    left: 20px;
    width: 150px;

    .text {
      font-size: 2rem;
      line-height: 30px;

      @media (min-width: $breakpoint-sm) and (max-width: ($breakpoint-xl - 1px)) {
        font-size: 7.8px;
        line-height: 10px;
        width: 315px;
        text-indent: 5px;

      }

      span {
        font-weight: 700;
      }
    }

    .subtitle {
      font-size: 1rem;

      @media (min-width: $breakpoint-sm) and (max-width: ($breakpoint-xl - 1px)) {
        font-size: 0.8rem;
        line-height: 15px;
      }
    }
  }
  .content3 {
    position: absolute;
    text-align: justify;
    top: 435px;
    left: 20px;
    width: 150px;

    .text {
      font-size: 2rem;
      line-height: 30px;

      @media (min-width: $breakpoint-sm) and (max-width: ($breakpoint-xl - 1px)) {
        font-size: 7.8px;
        line-height: 10px;
        text-indent: 5px;
        width: 315px;
      }

      span {
        font-weight: 700;
      }
    }

    .subtitle {
      font-size: 1rem;

      @media (min-width: $breakpoint-sm) and (max-width: ($breakpoint-xl - 1px)) {
        font-size: 0.8rem;
        line-height: 15px;
      }
    }
  }
}
</style>

<template>
  <div>
    <div style="display: none">
      <div id="p13t">{{ $t("p13.title") }}</div>
      <div id="p13s">{{ $t("p13.subtitle") }}</div>
      <div id="p13p1">{{ $t("p13.paragraph1") }}</div>
      <div id="p13p2">{{ $t("p13.paragraph2") }}</div>
      <div id="p13p3">{{ $t("p13.paragraph3") }}</div>
    </div>
    <div class="content1">
      <div id="p13t_" class="title"></div>
    </div>
    <div class="content">
      <div id="p13s_" class="title"></div>
    </div>
    <div class="content2">
      <div id="p13p1_" class="text"></div>
    </div>
    <div class="content3">
      <div id="p13p2_" class="text"></div>
      <div id="p13p3_" class="text"></div>
    </div>
  </div>
</template>

<script>
export default {
  name: "Page13",
  mounted() {
    let ref = this;
    ref.processText("p13t");
    ref.processText("p13s");
    ref.processText("p13p1");
    ref.processText("p13p2");
    ref.processText("p13p3");
    window
      .jQuery("body")
      .on(
        "DOMSubtreeModified",
        "#p13t,#p13s,#p13p1,#p13p2,#p13p3",
        function () {
          ref.processText(window.jQuery(this).attr("id"));
        }
      );
  },
  methods: {
    processText(id) {
      let text = document.getElementById(id).textContent;
      let r = text.split(".");
      document.getElementById(id + "_").innerHTML = "";
      window.jQuery.each(r, function (i, w) {
        var node = document.createElement("span");
        var textnode = document.createTextNode(
          w + (id.slice(-1) == "t" || id.slice(-1) == "s" ? "" : ".")
        );
        node.appendChild(textnode);
        document.getElementById(id + "_").appendChild(node);
      });
    },
  },
};
</script>