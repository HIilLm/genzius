<style lang="scss">
.p11 {
  background-image: url("/img/pages/g-10.webp");
  background-position: center;
  background-repeat: no-repeat;
  background-size: cover;
  position: relative;
  // TEMPLATE 
      // @media (min-width: $breakpoint-xl) { // LAPTOP XL
       
      // }

      // @media (min-width:$breakpoint-lg) and (max-width:($breakpoint-xl - 1px )) { LAPTOP LARGE
        
      // }

      // @media (min-width:$breakpoint-md) and (max-width: ($breakpoint-lg - 1px)) { TABLET
        
      // }
      
      // @media (min-width: $breakpoint-sm) and (max-width: 480px) { HP
        
      // }
  //TEMPLATE
  .content1 {
    color: #fff;
    position: absolute;
    top: 40px;
    left: 75px;
    width: 150px;

    @media (min-width: $breakpoint-sm) and (max-width: ($breakpoint-xl - 1px)) {
      left: 64px;
    }

    @media (min-width: $breakpoint-xl) { // LAPTOP XL
      left: 115px;
      top: 50px;
    }

    .title {
      font-size: 2rem;
      line-height: 30px;

      @media (min-width: $breakpoint-sm) and (max-width: ($breakpoint-xl - 1px)) {
        font-size: 20px;
        line-height: 25px;
        width: 500px;
      }

      @media (min-width: $breakpoint-xl) { // LAPTOP XL
        font-size: 25px;
        width: 500px;
      }

      span {
        font-weight: 800;
      }
    }
  }

  .content2 {
    color: #fff;
    position: absolute;
    text-align: justify;
    top: 85px;
    left: 30px;
    width: 150px;

    @media (min-width: $breakpoint-xl) { // LAPTOP XL
      top: 100px;
      left: 45px;
    }

    @media (min-width: $breakpoint-sm) and (max-width: ($breakpoint-xl - 1px)) {
      left: 35px;
      top: 75px;
    }
    @media (min-width: $breakpoint-lg) and (max-width: ($breakpoint-xl - 1px)) {
      top: 85px;
      left: 40px;
    }

    .text {
      font-size: 2rem;
      line-height: 30px;

      @media (min-width: $breakpoint-sm) and (max-width: ($breakpoint-xl - 1px)) {
        font-size: 7.2px;
        line-height: 9px;
        width: 265px;
      }

      @media (min-width: $breakpoint-xl) { // LAPTOP XL
        font-size: 10px;
        line-height: 15px;
        width: 405px;
      }

      span {
        font-weight: 300;
      }
    }
  }

  .content3 {
    color: #fff;
    position: absolute;
    text-align: justify;
    top: 150px;
    left: 30px;
    width: 150px;

    @media (min-width: $breakpoint-xl) { // LAPTOP XL
      top: 190px;
      left: 45px;
    }

    @media (min-width: $breakpoint-sm) and (max-width: ($breakpoint-xl - 1px)) {
      left: 35px;
      top: 133px;
    }
    @media (min-width: $breakpoint-lg) and (max-width: ($breakpoint-xl - 1px)) {
      top: 140px;
      left: 40px;
    }

    .text {
      @media (min-width: $breakpoint-xl) { // LAPTOP XL
        font-size: 10px;
        line-height: 15px;
        width: 405px;
      }

      font-size: 2rem;
      line-height: 30px;

      @media (min-width: $breakpoint-sm) and (max-width: ($breakpoint-xl - 1px)) {
        font-size: 7.2px;
        line-height: 10px;
        width: 265px;
      }

      span {
        font-weight: 400;
      }
    }
  }

  .content4 {
    color: #fff;
    position: absolute;
    text-align: justify;
    top: 240px;
    left: 30px;
    width: 150px;

    @media (min-width: $breakpoint-xl) { // LAPTOP XL
      top: 320px;
      left: 45px;
    }

    @media (min-width: $breakpoint-sm) and (max-width: ($breakpoint-xl - 1px)) {
      left: 35px;
      top: 217px;
    }
    @media (min-width: $breakpoint-lg) and (max-width: ($breakpoint-xl - 1px)) {
      top: 230px;
      left: 40px;
    }

    .text {
      @media (min-width: $breakpoint-xl) { // LAPTOP XL
        font-size: 10px;
        line-height: 15px;
        width: 405px;
      }

      font-size: 2rem;
      line-height: 30px;

      @media (min-width: $breakpoint-sm) and (max-width: ($breakpoint-xl - 1px)) {
        font-size: 7.2px;
        line-height: 10px;
        width: 265px;
      }

      span {
        font-weight: 400;
      }
    }
  }

  .content5 {
    color: #fff;
    position: absolute;
    text-align: justify;
    top: 310px;
    left: 30px;
    width: 150px;

    @media (min-width: $breakpoint-xl) { // LAPTOP XL
      top: 410px;
      left: 45px;
    }

    @media (min-width: $breakpoint-sm) and (max-width: ($breakpoint-xl - 1px)) {
      left: 35px;
      top: 280px;
    }
    @media (min-width: $breakpoint-lg) and (max-width: ($breakpoint-xl - 1px)) {
      top: 300px;
      left: 40px;
    }

    .text {
      font-size: 2rem;
      line-height: 30px;

      @media (min-width: $breakpoint-xl) { // LAPTOP XL
        font-size: 10px;
        line-height: 15px;
        width: 405px;
      }
      @media (min-width: $breakpoint-sm) and (max-width: ($breakpoint-xl - 1px)) {
        font-size: 7.2px;
        line-height: 10px;
        width: 265px;
      }

      span {
        font-weight: 400;
      }
    }
  }
}
</style>

<template>
  <div>
    <div style="display: none">
      <div id="p10p1">{{ $t("p10.paragraph1") }}</div>
      <div id="p10p2">{{ $t("p10.paragraph2") }}</div>
      <div id="p10p3">{{ $t("p10.paragraph3") }}</div>
      <div id="p10p4">{{ $t("p10.paragraph4") }}</div>
      <div id="p10p5">{{ $t("p10.paragraph5") }}</div>
    </div>

    <div class="content1">
      <div id="p10p1_" class="title"></div>
    </div>
    <div class="content2">
      <div id="p10p2_" class="text"></div>
    </div>
    <div class="content3">
      <div id="p10p3_" class="text"></div>
    </div>
    <div class="content4">
      <div id="p10p4_" class="text"></div>
    </div>
    <div class="content5">
      <div id="p10p5_" class="text"></div>
    </div>
  </div>
</template>

<script>
export default {
  name: "Page10",
  mounted() {
    let ref = this;
    ref.processText("p10p1");
    ref.processText("p10p2");
    ref.processText("p10p3");
    ref.processText("p10p4");
    ref.processText("p10p5");
    window
      .jQuery("body")
      .on("DOMSubtreeModified",
          "#p10p1,#p10p2,#p10p3,#p10p4,#p10p5,", 
          function () {
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