<style lang="scss">
.p2 {
  background-image: url("/img/pages/REV-03.jpg");
  background-position: center;
  background-repeat: no-repeat;
  background-size: cover;
  position: relative;

  .content1{
    color: #ffffff;
    // position: absolute;
    // top: 110px;
    // left: 20px;
    

    // mengatur posisi teks dari atas
    @media (min-width: $breakpoint-lg) and (max-width: ($breakpoint-xl - 1px)) {
      top: 50px;
    }

    @media (min-width: 481px) and (max-width: ($breakpoint-lg - 1px)) {
      top: 215px;
    }

    @media (min-width: $breakpoint-sm) and (max-width: 480px) {
      top: 165px;
    }

    .title {
      // memisahkan title dengan paragraf
      text-align: center;
      margin-bottom: 5px;
      text-align: left;
      margin-left: 10px;
      margin-top: 50px;

      @media (min-width: $breakpoint-sm) and (max-width: 480px) {
        margin-bottom: 0px;
      }

      span {
        font-weight: 700;
        font-size: 3rem;

        @media (min-width: $breakpoint-lg) and (max-width: ($breakpoint-xl - 1px)) {
          font-size: 2rem;
        }

        @media (min-width: 481px) and (max-width: ($breakpoint-lg - 1px)) {
          font-size: 1.6rem;
        }

        @media (min-width: $breakpoint-sm) and (max-width: 480px) {
          margin-bottom: 0px;
          font-size: 1.6rem;
        }
      }
    }

    .text {
      font-size: rem;
      text-align:left;
      line-height: 20px;
      padding-left: 35px;
      padding-right: 10px;

      @media (min-width: $breakpoint-lg) and (max-width: ($breakpoint-xl - 1px)) {
        font-size: 2rem;
        line-height: 10px;
      }

      @media (min-width: 481px) and (max-width: ($breakpoint-lg - 1px)) {
        font-size: 0.7rem;
        line-height: 12px;
      }

      @media (min-width: $breakpoint-sm) and (max-width: 480px) {
        font-size: 0.5rem;
        line-height: 9px;
      }
    }
  }
  .content2 {
    color: #ffffff;
    position: absolute;
    top: 228px;
    width: 264px;
    left: 215px;
    font-size: 0.7rem;
    text-align: justify;

    @media (min-width: $breakpoint-lg) and (max-width: ($breakpoint-xl - 1px)) {
      top: 10px;
      width: 250px;
      left: 90px;
      font-size: 0.6rem;
    }

    @media (min-width: 481px) and (max-width: ($breakpoint-lg - 1px)) {
      top: 202px;
      width: 210px;
      left: 185px;
      font-size: 0.65rem;
    }

    @media (min-width: $breakpoint-sm) and (max-width: 480px) {
      top: 134px;
      width: 177px;
      left: 141px;
      font-size: 0.5rem;
    }

    .text1,
    .text2,
    .text3 {
      line-height: 14px;
      margin-top: 5px;

      @media (min-width: $breakpoint-lg) and (max-width: ($breakpoint-xl - 1px)) {
        line-height: 10px;
      }

      @media (min-width: 481px) and (max-width: ($breakpoint-lg - 1px)) {
        line-height: 11px;
      }

      @media (min-width: $breakpoint-sm) and (max-width: 480px) {
        line-height: 11px;
      }
    }

    .text2,
    .text3 {
      text-indent: 10px;
    }

    .text1::first-letter {
      color: #ffffff;
      font-size: 3rem;
      float: left;
      line-height: 40px;
    }
  }
  .content2 {
    color: #ffffff;
    position: absolute;
    top: 228px;
    width: 264px;
    left: 215px;
    font-size: 0.7rem;
    text-align: justify;

    @media (min-width: $breakpoint-lg) and (max-width: ($breakpoint-xl - 1px)) {
      top: 10px;
      width: 250px;
      left: 90px;
      font-size: 0.6rem;
    }

    @media (min-width: 481px) and (max-width: ($breakpoint-lg - 1px)) {
      top: 202px;
      width: 210px;
      left: 185px;
      font-size: 0.65rem;
    }

    @media (min-width: $breakpoint-sm) and (max-width: 480px) {
      top: 134px;
      width: 177px;
      left: 141px;
      font-size: 0.5rem;
    }

    .text1,
    .text2,
    .text3 {
      line-height: 14px;
      margin-top: 5px;

      @media (min-width: $breakpoint-lg) and (max-width: ($breakpoint-xl - 1px)) {
        line-height: 10px;
      }

      @media (min-width: 481px) and (max-width: ($breakpoint-lg - 1px)) {
        line-height: 11px;
      }

      @media (min-width: $breakpoint-sm) and (max-width: 480px) {
        line-height: 11px;
      }
    }

    .text2,
    .text3 {
      text-indent: 10px;
    }
  }
}
</style>

<template>
  <div>
    <div style="display: none">
      <div id="p3t">{{ $t("p3.title") }}</div>
      <div id="p3s">{{ $t("p3.subtitle") }}</div>
      <div id="p3p1">{{ $t("p3.paragraph1") }}</div>
      <div id="p3p2">{{ $t("p3.paragraph2") }}</div>
      <div id="p3p3">{{ $t("p3.paragraph3") }}</div>
    </div>

    <div class="content2">
      <div id="p3p1_" class="text1"></div>
      <div id="p3p2_" class="text2"></div>
      <div id="p3p3_" class="text3"></div>
    </div>
    <div class="content3">

    </div>
  </div>
</template>

<script>
import jQuery from "jquery";

window.jQuery = jQuery;

export default {
  name: "Page1",
  mounted() {
    let ref = this;
    ref.processText("p1t");
    ref.processText("p1p1");
    window.jQuery("body").on("DOMSubtreeModified", "#p1t, #p1p1", function () {
      ref.processText(window.jQuery(this).attr("id"));
    });
  },
  methods: {
    processText(id) {
      let text = document.getElementById(id).textContent;
      let r = text.split(".");
      document.getElementById(id + "_").innerHTML = "";
      window.jQuery.each(r, function (i, w) {
        var node = document.createElement("span");
        console.log(id.slice(-1));
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