<style lang="scss">
.p2 {
  background-image: url("/img/pages/g-01.webp");
  background-position: center;
  background-repeat: no-repeat;
  background-size: cover;
  position: relative;

  .contentb {
    color: #ffffff;
    .title {
      text-align: center;
      background-color: orangered;
      width: fit-content;

      // TEMPLATE 
      // @media (min-width: $breakpoint-xl) { // LAPTOP XL
       
      // }

      // @media (min-width:$breakpoint-lg) and (max-width:($breakpoint-xl - 1px )) { LAPTOP LARGE
        
      // }

      // @media (min-width:$breakpoint-md) and (max-width: ($breakpoint-lg - 1px)) { TABLET
        
      // }
      
      // @media (min-width: $breakpoint-sm) and (max-width: 600px) { HP
        
      // }
      //TEMPLATE

      @media (min-width: $breakpoint-xl) {
        margin-top: 40px;
        margin-left: 120px;
      }

      @media (min-width:$breakpoint-lg) and (max-width:($breakpoint-xl - 1px )) {
      
      }

      @media (min-width:$breakpoint-md) and (max-width: ($breakpoint-lg - 1px)) {
        
      }
      
      @media (min-width: $breakpoint-sm) and (max-width: 600px) {
        margin-top: 40px;
        margin-left: 80px;
      }
      
      span {
        margin: 0px 5px;
        font-weight: 700;
        @media (min-width: $breakpoint-xl) {
          font-size: 21px;
        }

        @media (min-width: $breakpoint-sm) and (max-width: 600px) {
          font-size: 12px;
        }
      }
    }
  }

  .content1 {
    color: #ffffff;

    @media (min-width: $breakpoint-sm) and (max-width: 600px) {
      top: 162px;
    }

    .title {
      text-align: center;
      // margin-bottom: 5px;
      width: fit-content;
      background-color: orangered;
      
      @media (min-width:  $breakpoint-xl) { //LAPTOP LG
        margin-top: 15px;
        margin-left: 120px;
      }
      
      @media (min-width:$breakpoint-lg) and (max-width: ($breakpoint-xl - 1px)) { //LAPTOP MD
        width: 225px;
      }

      @media (min-width: $breakpoint-sm) and (max-width: 600px) { //HP
        margin-top: 4px;
        margin-left: 80px;
      }

      span {
        font-weight: 700;
        font-size: 25px;
        @media (min-width: $breakpoint-xl) {
          font-size: 21px;
          margin: 0px 5px;
        }
        @media (min-width:$breakpoint-lg) and (max-width: 1300px)  {
          margin-left: 0;
        }
        @media (min-width: $breakpoint-sm) and (max-width: 600px) {
          font-size: 12px;
          margin: 0px 5px;
        }
      }
    }
  }

  .content2 {
    ::first-letter {
      color: orange;
      font-size: 2rem;
      font-weight: 500;
      float: left;
      line-height: 20px;
      margin-left: 0px;
    }

    color: orange;
    position: absolute;
    text-align: justify;
    top: 105px;
    left: 120px;
    width: 200px;

    @media (min-width: $breakpoint-xl) {
      top: 135px;
    }

    @media (min-width: $breakpoint-sm) and (max-width: ($breakpoint-md - 1px)) {
      left: 80px;
      top: 105px;
    }

    .text {
      font-size: 10px;
      line-height: 12px;

      @media (min-width: $breakpoint-sm) and (max-width: ($breakpoint-md - 1px)) {
        font-size: 6px;
        line-height: 7px;
        width: 140px;

      }

      span {
        font-weight: 700;

        @media (min-width: $breakpoint-sm) and (max-width: ($breakpoint-md - 1px)) {
          font-weight: 500;
        }

        @media (min-width: $breakpoint-xl) {
          font-weight: 500;
        }
      }
    }
  }

  .content3 {
    color: orange;
    position: absolute;
    text-align: justify;
    width: 353px;

    @media (min-width:$breakpoint-lg) and (max-width: 1300px)  {
      margin-top: 5px;
      margin-left: 10px;
    }

    @media (min-width: $breakpoint-xl) {
      top: 257px;
      left: 120px;
    }

    @media (min-width: $breakpoint-sm) and (max-width: ($breakpoint-md - 1px)) {
      left: 80px;
      top: 175px;
    }

    .text {
      font-size: 10px;
      line-height: 12px;

      @media (min-width: $breakpoint-sm) and (max-width: ($breakpoint-md - 1px)) {
        font-size: 6px;
        line-height: 10px;
        width: 240px;
      }

      span {
        @media (min-width: $breakpoint-sm) and (max-width: ($breakpoint-md - 1px)) {
          font-weight: 500;
        }

        @media (min-width: $breakpoint-xl) {
          font-weight: 500;
        }
      }
    }
  }

  .content4 {
    color: orange;
    position: absolute;
    text-align: justify;
    top: 340px;

    @media (min-width: $breakpoint-sm) and (max-width: ($breakpoint-md - 1px)) {
      top: 230px;
      left: 180px;
    }

    left: 260px;
    width: 200px;

    @media (min-width: $breakpoint-xl) {
      width: 212px;
    }

    .text {
      font-size: 10px;
      line-height: 12px;

      @media (min-width: $breakpoint-sm) and (max-width: ($breakpoint-md - 1px)) {
        font-size: 6px;
        line-height: 10px;
        width: 140px;

      }

      span {
        font-weight: 700;

        @media (min-width: $breakpoint-sm) and (max-width: ($breakpoint-md - 1px)) {
          font-weight: 500;

        }

        @media (min-width: $breakpoint-xl) {
          font-weight: 500;
        }
      }
    }
  }

  .content5 {
    color: orange;
    position: absolute;
    text-align: justify;
    top: 440px;
    left: 80px;
    width: 75%;

    @media (min-width: $breakpoint-xl) {
        width: 353px;
        left: 115px;
    }

    @media (min-width: $breakpoint-sm) and (max-width: ($breakpoint-md - 1px)) {
      top: 300px;
      left: 80px;
    }

    .text {
      font-size: 10px;
      line-height: 14px;
      @media (min-width: $breakpoint-sm) and (max-width: ($breakpoint-md - 1px)) {
        font-size: 6px;
        line-height: 10px;
        width: 235px;
      }

      span {
        font-weight: 700;
        @media (min-width: $breakpoint-sm) and (max-width: ($breakpoint-md - 1px)) {
          font-weight: 500;
        }
        @media (min-width: $breakpoint-xl) {
          font-weight: 500;
        }
      }
    }
  }

  .content6 {
    color: orange;
    position: absolute;
    text-align: justify;
    top: 485px;
    left: 115px;
    width: 215px;

    @media (min-width: $breakpoint-sm) and (max-width: ($breakpoint-md - 1px)) {
      top: 330px;
      left: 80px;
    }

    .text {
      font-size: 10px;
      line-height: 12px;

      @media (min-width: $breakpoint-sm) and (max-width: ($breakpoint-md - 1px)) {
        font-size: 6px;
        line-height: 7px;
        width: 130px;

      }

      span {
        font-weight: 700;
        @media (min-width: $breakpoint-sm) and (max-width: ($breakpoint-md - 1px)) {
          font-weight: 500;
        }
        @media (min-width: $breakpoint-xl) {
          font-weight: 500;
        }
      }
    }
  }

  .content7 {
    color: orange;
    position: absolute;
    text-align: justify;
    top: 595px;
    left: 115px;
    width: 355px;

    @media (min-width: $breakpoint-sm) and (max-width: ($breakpoint-md - 1px)) {
      top: 400px;
      left: 80px;
    }

    .text {
      font-size: 10px;
      line-height: 12px;

      @media (min-width: $breakpoint-sm) and (max-width: ($breakpoint-md - 1px)) {
        font-size: 6px;
        line-height: 10px;
        width: 235px;

      }

      span {
        font-weight: 700;

        @media (min-width: $breakpoint-sm) and (max-width: ($breakpoint-md - 1px)) {
          font-weight: 500;
        }
        @media (min-width: $breakpoint-xl) {
          font-weight: 500;
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
      <div id="p1p6">{{ $t("p1.paragraph6") }}</div>
      <div id="p1p7">{{ $t("p1.paragraph7") }}</div>
    </div>
    <div class="contentb">
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