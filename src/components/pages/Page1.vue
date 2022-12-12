<style lang="scss">
.p2 {
  background-image: url("/img/pages/01.jpg");
  background-position: center;
  background-repeat: no-repeat;
  background-size: cover;
  position: relative;

  .content{
    color:#ffffff;

    // position: absolute;
    // top: 110px;
    // left: 20px;
    
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
      width: 200px;
      background-color: orangered;
      margin-left: 90px;
      margin-top: 30px;

      @media (min-width: $breakpoint-sm) and (max-width: 480px) {
        margin-bottom: 0px;
      }

      span {
        font-weight: 700;
        font-size: 1px;

        @media (min-width: $breakpoint-lg) and (max-width: ($breakpoint-xl - 1px)) {
          font-size: 18px;
          // margin-left: 70px;
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
  .content2 {
    ::first-letter{
      color: orange;
      font-size: 2rem;
      font-weight: 500;
      float:left;
      line-height: 20px;
      margin-left: 0px;
    }
    color: orange;
    position: absolute;
    text-align: justify;
    top: 105px;
    left: 85px;
    width: 150px;

    .text {
      font-size: 2rem;
      line-height: 30px;

      @media (min-width: $breakpoint-sm) and (max-width: ($breakpoint-xl - 1px)) {
        font-size: 6px;
        line-height: 10px;
        width: 150px;

      }

      span {
        font-weight: 700;
      }
    }
  }
  .content6 {
    color: orange;
    position: absolute;
    text-align: justify;
    top: 348px;
    left: 85px;
    width: 150px;

    .text {
      font-size: 2rem;
      line-height: 30px;

      @media (min-width: $breakpoint-sm) and (max-width: ($breakpoint-xl - 1px)) {
        font-size: 6px;
        line-height: 10px;
        width: 150px;

      }

      span {
        font-weight: 700;
      }
    }
  }
  .content4 {
    color: orange;
    position: absolute;
    text-align: justify;
    top: 240px;
    left: 190px;
    width: 150px;

    .text {
      font-size: 2rem;
      line-height: 30px;

      @media (min-width: $breakpoint-sm) and (max-width: ($breakpoint-xl - 1px)) {
        font-size: 6px;
        line-height: 10px;
        width: 150px;

      }

      span {
        font-weight: 700;
      }
    }
  }
  .content5 {
    color: orange;
    position: absolute;
    text-align: justify;
    top: 315px;
    left: 85px;
    width: 150px;

    .text {
      font-size: 2rem;
      line-height: 30px;

      @media (min-width: $breakpoint-sm) and (max-width: ($breakpoint-xl - 1px)) {
        font-size: 6px;
        line-height: 10px;
        width: 255px;

      }

      span {
        font-weight: 700;
      }
    }
  }
  .content7 {
    color: orange;
    position: absolute;
    text-align: justify;
    top: 430px;
    left: 85px;
    width: 150px;

    .text {
      font-size: 2rem;
      line-height: 30px;

      @media (min-width: $breakpoint-sm) and (max-width: ($breakpoint-xl - 1px)) {
        font-size: 6px;
        line-height: 10px;
        width: 255px;

      }

      span {
        font-weight: 700;
      }
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
    color:#ffffff;
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
      width: 240px;
      background-color: orangered;
      margin-left: 90px;
      margin-top: 10px;

      @media (min-width: $breakpoint-sm) and (max-width: 480px) {
        margin-bottom: 50px;
      }

      span {
        font-weight: 700;
        font-size: 1px;

        @media (min-width: $breakpoint-lg) and (max-width: ($breakpoint-xl - 1px)) {
          font-size: 18px;
          // margin-left: 70px;
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
  .content3 {
    color: orange;
    position: absolute;
    text-align: justify;
    top: 181px;
    left: 5px;
    width: 150px;

    .text {
      font-size: 2rem;
      line-height: 30px;

      @media (min-width: $breakpoint-sm) and (max-width: ($breakpoint-xl - 1px)) {
        font-size: 6px;
        line-height: 10px;
        width: 353px;

      }

      span {
        font-weight: 700;
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
      <div id="p1p6">{{ $t("p1.paragraph6") }}</div>
      <div id="p1p7">{{ $t("p1.paragraph7") }}</div>
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
    </div>
    <div class="content4">
      <div id="p1p4_" class="text"></div>
    </div>
    <div class="content5">
      <div id="p1p5_" class="text"></div>
    </div>
    <div class="content6">
      <div id="p1p6_" class="text"></div>
    </div>
    <div class="content7">
      <div id="p1p7_" class="text"></div>
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
    ref.processText("p1p6");
    ref.processText("p1p7");
    window.jQuery("body").on("DOMSubtreeModified", "#p1t, #p1p1, #p1p2, #p1p3, #p1p4, #p1p5, #p1p6, #p1p7", function () {
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