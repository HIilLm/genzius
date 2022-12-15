<style lang="scss">
.p8 {
  background-image: url("/img/pages/07.jpg");
  background-position: center;
  background-repeat: no-repeat;
  background-size: cover;
  position: relative;

  .content1 {
    position: absolute;
    top: 204px;
    left: 60px;
    width: 270px;

    @media (min-width:1440px) {
      top: 55px;
      left: 270px;
    }

    @media (min-width: $breakpoint-lg) and (max-width: ($breakpoint-xl - 1px)) {
      top: 40px;
      left: 190px;
      width: 197px;
    }

    @media (min-width: 481px) and (max-width: ($breakpoint-lg - 1px)) {
      top: 172px;
      left: 50px;
      width: 211px;
    }

    @media (min-width: $breakpoint-sm) and (max-width: 480px) {
      top: 20px;
      left: 180px;
      width: 197px;
    }

    .title {
      span {
        color: black;
        font-weight: 600;
        font-size: 1.1rem;
        line-height: 1px;

        @media (min-width: 1440px) {
          font-size: 30px;
        }

        @media (min-width: $breakpoint-lg) and (max-width: ($breakpoint-xl - 1px)) {
          font-size:20px;
        }

        @media (min-width: 481px) and (max-width: ($breakpoint-lg - 1px)) {
          font-size: 0.8rem;
        }

        @media (min-width: $breakpoint-sm) and (max-width: 480px) {
          font-size: 20px;
        }
      }
    }
  }

  .content2 {
    position: absolute;
    top: 263px;
    left: 28px;
    width: 240px;
    text-align: justify;
    line-height: 13px;
    font-size: 0.7rem;
    font-weight: 800;
    @media (min-width:1440px) {
      top: 90px;
      left: 260px;
      width: 430px;
      font-size: 20px;
      text-align: justify;
    }

    @media (min-width: $breakpoint-lg) and (max-width: ($breakpoint-xl - 1px)) {
      top: 60px;
      left: 170px;
    }

    @media (min-width: 481px) and (max-width: ($breakpoint-lg - 1px)) {
      top: 229px;
      left: 27px;
      width: 207px;
    }

    @media (min-width: $breakpoint-sm) and (max-width: 480px) {
      top: 40px;
      left: 155px;
      width: 250px;
    }

    .text {
      // font-size: 0.7rem;

      @media (min-width: $breakpoint-lg) and (max-width: ($breakpoint-xl - 1px)) {
        font-size: 16px;
        line-height: 9px;
      }

      @media (min-width: 481px) and (max-width: ($breakpoint-lg - 1px)) {
        font-size: 0.65rem;
        line-height: 11px;
      }

      @media (min-width: $breakpoint-sm) and (max-width: 480px) {
        font-size: 17px;
      }
    }
  }
  .content3 {
    ::first-letter{
      color:orangered;
      font-size: 2rem;
      font-weight: 600;
      float:left;
      line-height: 15px;
    }
    color: orangered;
    position: absolute;
    top: 263px;
    left: 28px;
    width: 240px;
    text-align: justify;
    font-size: 0.7rem;
    @media (min-width:1440px) {
      color: orangered;
      top: 130px;
      left: 240px;
      width: 430px;
      font-size: 11px;
      text-align: justify;
    }

    @media (min-width: $breakpoint-lg) and (max-width: ($breakpoint-xl - 1px)) {
      top: 90px;
      left: 170px;
      width: 170px;
    }

    @media (min-width: 481px) and (max-width: ($breakpoint-lg - 1px)) {
      top: 229px;
      left: 27px;
      width: 207px;
    }

    @media (min-width: $breakpoint-sm) and (max-width: 480px) {
      top: 65px;
      left: 155px;
      width: 166px;
    }

    .text {
      @media (min-width:1440px) {
      color: orangered;
      top: 100px;
      left: 30px;
      width: 230px;
      font-size: 11px;
      text-align: justify;
      line-height: 13px;
 
    }
      font-size: 0.7rem;

      @media (min-width: $breakpoint-lg) and (max-width: ($breakpoint-xl - 1px)) {
        font-size: 8px;
        line-height: 9px;
      }

      @media (min-width: 481px) and (max-width: ($breakpoint-lg - 1px)) {
        font-size: 0.65rem;
        line-height: 11px;
      }

      @media (min-width: $breakpoint-sm) and (max-width: 480px) {
        font-size: 7.3px;
        line-height: 9px;
      }
    }
  }
  .content4 {
    color: orangered;
    position: absolute;
    top: 263px;
    left: 28px;
    width: 240px;
    text-align: justify;
    line-height: 13px;
    font-size: 0.7rem;
    @media (min-width:1440px) {
      color: orangered;
      top: 340px;
      left: 240px;
      width: 430px;
      font-size: 11px;
      text-align: justify;
    }

    @media (min-width: $breakpoint-lg) and (max-width: ($breakpoint-xl - 1px)) {
      top: 230px;
      left: 170px;
      width: 170px;
    }

    @media (min-width: 481px) and (max-width: ($breakpoint-lg - 1px)) {
      top: 229px;
      left: 27px;
      width: 207px;
    }

    @media (min-width: $breakpoint-sm) and (max-width: 480px) {
      top: 200px;
      left: 155px;
      width: 166px;
    }

    .text {
      font-size: 0.7rem;
      @media (min-width:1440px) {
      color: orangered;
      top: 100px;
      left: 30px;
      width: 230px;
      font-size: 11px;
      text-align: justify;
      line-height: 13px;

    }

      @media (min-width: $breakpoint-lg) and (max-width: ($breakpoint-xl - 1px)) {
        font-size: 8px;
        line-height: 9px;
      }

      @media (min-width: 481px) and (max-width: ($breakpoint-lg - 1px)) {
        font-size: 0.65rem;
        line-height: 11px;
      }

      @media (min-width: $breakpoint-sm) and (max-width: 480px) {
        font-size: 7.3px;
        line-height: 9px;
      }
    }
  }
  .content5 {
    color: orangered;
    position: absolute;
    top: 263px;
    left: 28px;
    width: 240px;
    text-align: justify;
    line-height: 13px;
    font-size: 0.7rem;
    @media (min-width:1440px) {
      color: orangered;
      top: 470px;
      left: 240px;
      width: 430px;
      font-size: 11px;
      text-align: justify;
    }
    @media (min-width: $breakpoint-lg) and (max-width: ($breakpoint-xl - 1px)) {
      top: 315px;
      left: 170px;
      width: 170px;
    }

    @media (min-width: 481px) and (max-width: ($breakpoint-lg - 1px)) {
      top: 229px;
      left: 27px;
      width: 207px;
    }

    @media (min-width: $breakpoint-sm) and (max-width: 480px) {
      top: 285px;
      left: 155px;
      width: 166px;
    }

    .text {
      @media (min-width:1440px) {
      color: orangered;
      top: 100px;
      left: 30px;
      width: 230px;
      font-size: 10px;
      text-align: justify;
      line-height: 11px;
    }
      font-size: 0.7rem;

      @media (min-width: $breakpoint-lg) and (max-width: ($breakpoint-xl - 1px)) {
        font-size: 8px;
        line-height: 9px;
      }

      @media (min-width: 481px) and (max-width: ($breakpoint-lg - 1px)) {
        font-size: 0.65rem;
        line-height: 11px;
      }

      @media (min-width: $breakpoint-sm) and (max-width: 480px) {
        font-size: 7.3px;
        line-height: 9px;
      }
    }
  }
}
</style>

<template>
  <div>
    <div style="display: none">
      <div id="p7t">{{ $t("p7.title") }}</div>
      <div id="p7p1">{{ $t("p7.paragraph1") }}</div>
      <div id="p7p2">{{ $t("p7.paragraph2") }}</div>
      <div id="p7p3">{{ $t("p7.paragraph3") }}</div>
      <div id="p7p4">{{ $t("p7.paragraph4") }}</div>
    </div>
    <div class="content1">
      <div id="p7t_" class="title"></div>
    </div>

    <div class="content2">
      <div id="p7p1_" class="text"></div>
    </div>
    <div class="content3">
      <div id="p7p2_" class="text"></div>
    </div>
    <div class="content4">    
      <div id="p7p3_" class="text"></div>
    </div>
    <div class="content5">
      <div id="p7p4_" class="text"></div>
    </div>
  </div>
</template>

<script>
export default {
  name: "Page7",
  mounted() {
    let ref = this;
    ref.processText("p7t");
    ref.processText("p7p1");
    ref.processText("p7p2");
    ref.processText("p7p3");
    ref.processText("p7p4");
    window
      .jQuery("body")
      .on("DOMSubtreeModified", "#p7t, #p7p1, #p7p2, #p7p3, #p7p4", function () {
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