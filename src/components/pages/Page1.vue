<style lang="scss">
.p2 {
  background-image: url("/img/pages/g-01.jpg");
  background-position: center;
  background-repeat: no-repeat;
  background-size: cover;
  position: relative;

  .content{
    color: #000000;

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
      margin-top: 35px;

      @media (min-width: $breakpoint-sm) and (max-width: 480px) {
        margin-bottom: 0px;
      }

      span {
        font-weight: 500;
        font-size: 1px;

        @media (min-width: $breakpoint-lg) and (max-width: ($breakpoint-xl - 1px)) {
          font-size: 20px;
          margin-left: 70px;
          background-color: #ffffff;
        }

        @media (min-width: 481px) and (max-width: ($breakpoint-lg - 1px)) {
          font-size: 20px;
          margin-left: 70px;
          background-color: #ffffff;
        }

        @media (min-width: $breakpoint-sm) and (max-width: 480px) {
          font-size: 20px;
          margin-left: 70px;
          background-color: #ffffff;
        }
      }
    }

    .text {
      font-size: 1px;
      text-align:left;
      line-height: 20px;
      padding-left: 35px;
      padding-right: 10px;

      @media (min-width: $breakpoint-lg) and (max-width: ($breakpoint-xl - 1px)) {
        font-size: 15px;
        line-height: 10px;
      }

      @media (min-width: 481px) and (max-width: ($breakpoint-lg - 1px)) {
        font-size: 15px;
        line-height: 10px;
      }

      @media (min-width: $breakpoint-sm) and (max-width: 480px) {
        font-size: 15px;
        line-height: 10px;
      }
    }
  }
  .content2{
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

    .text {
        font-size: 1px;
        text-align:justify;
        line-height: 20px;
        padding-left: 80px;
        padding-right: 20px;
        padding-top: 5px;

      @media (min-width: $breakpoint-lg) and (max-width: ($breakpoint-xl - 1px)) {
        font-size: 8.7px;
        line-height: 10px;
      }

      @media (min-width: 481px) and (max-width: ($breakpoint-lg - 1px)) {
        font-size: 8.7px;
        line-height: 10px;
      }

      @media (min-width: $breakpoint-sm) and (max-width: 480px) {
        font-size: 8.7px;
        line-height: 10px;
      }
    }
    .text::first-letter {
      color:#ffffff;
      font-size: 2rem;
      float: left;
      line-height: 20px;
    }
  }
  .content3{
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

    .text {
      font-size: 1px;
      text-align:justify;
      line-height: 20px;
      padding-left: 80px;
      padding-right: 20px;
      padding-top: 5px;

      @media (min-width: $breakpoint-lg) and (max-width: ($breakpoint-xl - 1px)) {
        font-size: 8.7px;
        line-height: 10px;
      }

      @media (min-width: 481px) and (max-width: ($breakpoint-lg - 1px)) {
        font-size: 8.7px;
        line-height: 10px;
      }

      @media (min-width: $breakpoint-sm) and (max-width: 480px) {
        font-size: 8.7px;
        line-height: 10px;
      }
    }
  }
  .content1{
    color: orangered;
    // position: absolute;
    // top: 110px;
    // left: 20px;
    

    // mengatur posisi teks dari atas
    @media (min-width: $breakpoint-lg) and (max-width: ($breakpoint-xl - 1px)) {
      top: 60px;
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
      margin-top: 10px;

      @media (min-width: $breakpoint-sm) and (max-width: 480px) {
        margin-bottom: 50px;
      }

      span {
        font-weight: 700;
        font-size: 1px;

        @media (min-width: $breakpoint-lg) and (max-width: ($breakpoint-xl - 1px)) {
          font-size: 18px;
          margin-left: 70px;
          background-color: #ffffff;
        }

        @media (min-width: 481px) and (max-width: ($breakpoint-lg - 1px)) {
          font-size: 18px;
          margin-left: 70px;
          background-color: #ffffff;
        }

        @media (min-width: $breakpoint-sm) and (max-width: 480px) {
          font-size: 18px;
          margin-left: 70px;
          background-color: #ffffff;
        }
      }
    }
  }
}
</style>

<template>
  <div>
    <div style="display: none">
      <div id="p1t">{{ $t("p1.title") }}</div>
      <div id="p1p1">{{ $t("p1.paragraph1") }}</div>
      <div id="p1p2">{{ $t("p1.paragraph2") }}</div>
      <div id="p1p3">{{ $t("p1.paragraph3") }}</div>
      <div id="p1p4">{{ $t("p1.paragraph4") }}</div>
      <div id="p1p5">{{ $t("p1.paragraph5") }}</div>
    </div>
    <div class="content">
      <div id="p1t_" class="title"></div>
    </div>
    <div class="content1">
      <div id="p1p1_" class="title"></div>
    </div>
    <div class="content2">
      <div id="p1p2_" class="text"></div>
    </div>
    <div class="content3">
      <div id="p1p3_" class="text"></div>
      <div id="p1p4_" class="text"></div>
      <div id="p1p5_" class="text"></div>
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
    ref.processText("p1p2");
    ref.processText("p1p3");
    ref.processText("p1p4");
    ref.processText("p1p5");
    window.jQuery("body").on("DOMSubtreeModified", "#p1t, #p1p1, #p1p2, #p1p3, #p1p4, #p1p5", function () {
      ref.processText(window.jQuery(this).attr("id"));
    });
  },
  methods: {
    processText(id) {
      let text = document.getElementById(id).textContent;
      let r = text.split("`");
      document.getElementById(id + "_").innerHTML = "";
      window.jQuery.each(r, function (i, w) {
        var node = document.createElement("span");
        console.log(id.slice(-1));
        var textnode = document.createTextNode(
          w + (id.slice(-1) == "t" || id.slice(-1) == "s" ? "" : "")
        );
        node.appendChild(textnode);
        document.getElementById(id + "_").appendChild(node);
      });
    },
  },
};
</script>