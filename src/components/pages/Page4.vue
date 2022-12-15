<style lang="scss">
  // @import url('https://fonts.cdnfonts.com/css/austrian');
.p5 {
  background-image: url("/img/pages/g-04.webp");
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
    position: absolute;
    top: 105px;
    left: 33px; 
    padding-left: 15px;
    width: 140px;
    @media (min-width: $breakpoint-sm) and (max-width: ($breakpoint-xl - 1px)) {
      top: 100px;
      left: 28px;
    }
    @media (min-width: $breakpoint-xl) { // LAPTOP XL
      width: 350px;
      left: 65px; 
      top: 145px;
    }
    .title {
      font-size: 2rem;
      line-height: 30px;
      
      @media (min-width: $breakpoint-xl) { // LAPTOP XL
        font-size: 30px;
      }
      
      @media (min-width: $breakpoint-sm) and (max-width: ($breakpoint-xl - 1px)) {
        font-size: 25px;
        line-height: 25px;
        width: 400px;
      }
      
      span {
        font-weight: 500;
        @media (min-width: $breakpoint-xl) { // LAPTOP XL
          // font-family: 'Austrian', sans-serif;
          font-weight: 700;
      }
        
      }
    }
  }
  .content2 {
    position: absolute;
    text-align: justify;
    top: 150px;
    left: 15px;
    width: 150px;
    @media (min-width: $breakpoint-sm) and (max-width: ($breakpoint-xl - 1px)) {
        top: 140px;
    }
    @media (min-width: $breakpoint-xl) { // LAPTOP XL
      top: 205px;
      left: 20px;
      width: 450px;
    }
    .text {
      font-size: 2rem;
      line-height: 30px;
      
      @media (min-width: $breakpoint-xl) { // LAPTOP XL
        font-size: 10px;
        line-height: 12px;
      }

      @media (min-width: $breakpoint-sm) and (max-width: ($breakpoint-xl - 1px)) {
        font-size: 7px;
        line-height: 7.8px;
        width: 302px;
      }

      span {
        @media (min-width: $breakpoint-sm) and (max-width: ($breakpoint-xl - 1px)) {
        font-weight: 500;
      }
      @media (min-width: $breakpoint-xl) { // LAPTOP XL
        font-weight: 500;
    }
        font-weight: 800;
      }
    }
  }
  .content3 {
    position: absolute;
    text-align: justify;
    top: 200px;
    left: 15px;
    width: 150px;
    @media (min-width: $breakpoint-xl) { // LAPTOP XL
      top: 270px;
      left: 20px;
      width: 450px;
    }
    @media (min-width: $breakpoint-sm) and (max-width: ($breakpoint-xl - 1px)) {
       top: 187px;
    }
    .text {
      font-size: 2rem;
      line-height: 30px;
      @media (min-width: $breakpoint-xl) { // LAPTOP XL
        font-size: 10px;
        line-height: 10px;
    }
      @media (min-width: $breakpoint-sm) and (max-width: ($breakpoint-xl - 1px)) {
        font-size: 7px;
        line-height: 7px;
        width: 302px;

      }

      span {
        @media (min-width: $breakpoint-sm) and (max-width: ($breakpoint-xl - 1px)) {
          font-weight: 500;
        }
        @media (min-width: $breakpoint-xl) { // LAPTOP XL
          font-weight: 500;
        }
        font-weight: 800;
      }
    }
  }
  .content4 {
    position: absolute;
    text-align: justify;
    top: 250px;
    left: 15px;
    width: 150px;
    @media (min-width: $breakpoint-xl) { // LAPTOP XL
      top: 325px;
      left: 20px;
    }
    @media (min-width: $breakpoint-sm) and (max-width: ($breakpoint-xl - 1px)) {
       top: 230px;
    }
    .text {
      font-size: 2rem;
      line-height: 30px;
      @media (min-width: $breakpoint-xl) { // LAPTOP XL
        font-size: 10px;
        line-height: 10px;
        width: 450px;
    }
      @media (min-width: $breakpoint-sm) and (max-width: ($breakpoint-xl - 1px)) {
        font-size: 7px;
        line-height: 7px;
        width: 302px;

      }

      span {
        font-weight: 800;
        @media (min-width: $breakpoint-sm) and (max-width: ($breakpoint-xl - 1px)) {
          font-weight: 500;
        }
        @media (min-width: $breakpoint-xl) { // LAPTOP XL
          font-weight: 500;
    }
      }
    }
  }
  .content5 {
    position: absolute;
    text-align: justify;
    top: 280px;
    left: 165px;
    width: 150px;
    @media (min-width: $breakpoint-sm) and (max-width: ($breakpoint-xl - 1px)) {
       top: 260px;
    }
    @media (min-width: $breakpoint-xl) { // LAPTOP XL
      top: 360px;
      left: 230px;
    }
    .text {
      font-size: 2rem;
      line-height: 30px;
      @media (min-width: $breakpoint-xl) { // LAPTOP XL
        font-size: 10px;
        }
      @media (min-width: $breakpoint-sm) and (max-width: ($breakpoint-xl - 1px)) {
        font-size: 7px;
        line-height: 9px;
        width: 320px;

      }

      span {
        font-weight: 800;
        @media (min-width: $breakpoint-xl) { // LAPTOP XL
          font-weight: 700;
        }
      }
    }
  }
  .content6 {
    position: absolute;
    text-align: center;
    top: 295px;
    left: 15px;
    width: 150px;
    @media (min-width: $breakpoint-xl) { // LAPTOP XL
      top: 382px;
      left: 50px;
    }
    @media (min-width: $breakpoint-sm) and (max-width: ($breakpoint-xl - 1px)) {
       top: 273px;
    }
    .text {
      font-size: 2rem;
      line-height: 30px;
      @media (min-width: $breakpoint-xl) { // LAPTOP XL
        font-size: 10px;
        line-height: 10px;
        width: 400px;
      }
      @media (min-width: $breakpoint-sm) and (max-width: ($breakpoint-xl - 1px)) {
        font-size: 7px;
        line-height: 9px;
        width: 302px;

      }

      span {
          font-weight: 800;
        @media (min-width: $breakpoint-sm) and (max-width: ($breakpoint-xl - 1px)) {
          font-weight: 500;
        }
        @media (min-width: $breakpoint-xl) { // LAPTOP XL
          font-weight: 500;
        }
      }
    }
  }
  .content7 {
    position: absolute;
    text-align: justify;
    top: 330px;
    left: 165px;
    width: 150px;
    @media (min-width: $breakpoint-xl) { // LAPTOP XL
      top: 415px;
      left: 230px;
    }
    @media (min-width: $breakpoint-sm) and (max-width: ($breakpoint-xl - 1px)) {
       top: 305px;
    }
    .text {
      font-size: 2rem;
      line-height: 30px;

      @media (min-width: $breakpoint-xl) { // LAPTOP XL
        font-size: 10px;
      }

      @media (min-width: $breakpoint-sm) and (max-width: ($breakpoint-xl - 1px)) {
        font-size: 7px;
        line-height: 9px;
        width: 320px;

      }

      span {
        font-weight: 800;
        @media (min-width: $breakpoint-xl) { // LAPTOP XL
          font-weight: 700;
        }
      }
    }
  }
  .content8 {
    position: absolute;
    text-align: center;
    top: 345px;
    left: 15px;
    width: 150px;
    @media (min-width: $breakpoint-sm) and (max-width: ($breakpoint-xl - 1px)) {
       top: 315px;
       
      }
      @media (min-width: $breakpoint-xl) { // LAPTOP XL
        top: 437px;
        left: 55px;
        width: 380px;
        }
    .text {
      font-size: 2rem;
      line-height: 30px;

      @media (min-width: $breakpoint-sm) and (max-width: ($breakpoint-xl - 1px)) {
        font-size: 7px;
        line-height: 9px;
        width: 310px;

      }
      @media (min-width: $breakpoint-xl) { // LAPTOP XL
        font-size: 10px;
        line-height: 10px;
        }

      span {
        font-weight: 800;
        @media (min-width: $breakpoint-sm) and (max-width: ($breakpoint-xl - 1px)) {
          font-weight: 500;
        }
        @media (min-width: $breakpoint-xl) { // LAPTOP XL
          font-weight: 500;
        }
      }
    }
  }
  .content9 {
    position: absolute;
    text-align: justify;
    top: 410px;
    left: 15px;
    width: 150px;
    @media (min-width: $breakpoint-xl) { // LAPTOP XL
      top: 530px;
      left: 20px;
      width: 450px;
    }
    @media (min-width: $breakpoint-sm) and (max-width: ($breakpoint-xl - 1px)) {
       top: 380px;
    }
    .text {
      font-size: 2rem;
      line-height: 30px;

      @media (min-width: $breakpoint-xl) { // LAPTOP XL
        font-size: 10px;
        line-height: 10px;
      }

      @media (min-width: $breakpoint-sm) and (max-width: ($breakpoint-xl - 1px)) {
        font-size: 7px;
        line-height: 7px;
        width: 302px;
      }

      span {
        font-weight: 800;
        @media (min-width: $breakpoint-sm) and (max-width: ($breakpoint-xl - 1px)) {
        font-weight: 500;
        }
        @media (min-width: $breakpoint-xl) { // LAPTOP XL
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
      <div id="p4p1">{{ $t("p4.paragraph1") }}</div>
      <div id="p4p2">{{ $t("p4.paragraph2") }}</div>
      <div id="p4p3">{{ $t("p4.paragraph3") }}</div>
      <div id="p4p4">{{ $t("p4.paragraph4") }}</div>
      <div id="p4p5">{{ $t("p4.paragraph5") }}</div>
      <div id="p4p6">{{ $t("p4.paragraph6") }}</div>
      <div id="p4p7">{{ $t("p4.paragraph7") }}</div>
      <div id="p4p8">{{ $t("p4.paragraph8") }}</div>
      <div id="p4p9">{{ $t("p4.paragraph9") }}</div>
    </div>
    <div class="content1">
      <div id="p4p1_" class="title"></div>
    </div>
    <div class="content2">
      <div id="p4p2_" class="text"></div>
    </div>
    <div class="content3">
      <div id="p4p3_" class="text"></div>
    </div>
    <div class="content4">
      <div id="p4p4_" class="text"></div>
    </div>
    <div class="content5">
      <div id="p4p5_" class="text"></div>
    </div>
    <div class="content6">
      <div id="p4p6_" class="text"></div>
    </div>
    <div class="content7">
      <div id="p4p7_" class="text"></div>
    </div>
    <div class="content8">
      <div id="p4p8_" class="text"></div>
    </div>
    <div class="content9">
      <div id="p4p9_" class="text"></div>
    </div>
  </div>
</template>

<script>
export default {
  name: "Page4",
  mounted() {
    let ref = this;
    ref.processText("p4p1");
    ref.processText("p4p2");
    ref.processText("p4p3");
    ref.processText("p4p4");
    ref.processText("p4p5");
    ref.processText("p4p6");
    ref.processText("p4p7");
    ref.processText("p4p8");
    ref.processText("p4p9");
    window
      .jQuery("body")
      .on("DOMSubtreeModified", "#p4p1, #p4p2, #p4p3, #p4p4,#p4p5,#p4p6,#p4p7,#p4p8,#p4p9", function () {
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