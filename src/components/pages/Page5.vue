<style lang="scss">
.p6 {
  background-image: url("/img/pages/g-05.webp");
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
      
      // @media (min-width: $breakpoint-sm) and (max-width: 600px) { HP
        
      // }
  //TEMPLATE
  .content1 {
    color: orange;
    position: absolute;
    top: 20px;
    left: 85px;
    padding-left: 15px;
    width: 140px;
    @media (min-width:1440px) {
      top: 40px;
      left: 100px;
      width: 300px;
      text-align: center;
    }
    @media (min-width: $breakpoint-sm) and (max-width: ($breakpoint-xl - 1px)) {
        left: 74px;
      }
      @media (min-width:$breakpoint-md) and (max-width: ($breakpoint-lg - 1px)) {
        left: 30px; 
        top: 25px;
        }
    .title {
      font-size: 2rem;
      line-height: 30px;
      @media (min-width:1440px) {
        line-height: 40px;
      }
      @media (min-width: $breakpoint-sm) and (max-width: ($breakpoint-xl - 1px)) {
        text-align: center;
        font-size: 20px;
        line-height: 30px;
        width: 160px;
      }

      @media (min-width:$breakpoint-md) and (max-width: ($breakpoint-lg - 1px)) {
        width: 260%;
        font-size: 2rem;
        line-height: 30px;
      }

      span {
        font-weight: 800;
      }
    }
  }
  .content2 {
    ::first-letter{
      color: black;
      font-size: 2rem;
      font-weight: 500;
      float:left;
      line-height: 25px;
      margin-left: 0px;
    }
    position: absolute;
    text-align: justify;
    top: 95px;
    left: 20px;
    width: 150px;
    @media (min-width:1440px) {
      top: 140px;
      left: 30px;
      width: 210px;
      text-align: justify;
    }

    @media (min-width:$breakpoint-md) and (max-width: ($breakpoint-lg - 1px)) {
      left: 25px; 
      top: 115px;
      }
    .text {
      font-size: 8px;
      line-height: 13px;

      @media (min-width: $breakpoint-sm) and (max-width: ($breakpoint-xl - 1px)) {
        font-size: 6px;
        line-height: 7.5px;
        width: 145px;
      }

      @media (min-width:$breakpoint-md) and (max-width: ($breakpoint-lg - 1px)) {
        width: 120%;
        font-size: 8.5px;
        line-height: 10px;
      }

      span {
        font-weight: 700;
        @media (min-width: $breakpoint-sm) and (max-width: ($breakpoint-xl - 1px)) {
          font-weight: 400;
        }
      }
    }
  }
  .content3 {
    position: absolute;
    text-align: justify;
    top: 210px;
    left: 20px;
    width: 150px;
    @media (min-width:1440px) {
      top: 290px;
      left: 30px;
      width: 210px;
      text-align: justify;
    }
    @media (min-width: $breakpoint-sm) and (max-width: ($breakpoint-xl - 1px)) {
      top: 190px;
    }

    @media (min-width:$breakpoint-md) and (max-width: ($breakpoint-lg - 1px)) {
      left: 25px; 
      top: 245px;
      }
    .text {
      font-size: 8px;
      line-height: 15px;

      @media (min-width: $breakpoint-sm) and (max-width: ($breakpoint-xl - 1px)) {
        font-size: 6px;
        line-height: 10px;
        width: 145px;
      }

      @media (min-width:$breakpoint-md) and (max-width: ($breakpoint-lg - 1px)) {
        width: 120%;
        font-size: 8.5px;
        line-height: 10px;
      }

      span {
        font-weight: 700;
        @media (min-width: $breakpoint-sm) and (max-width: ($breakpoint-xl - 1px)) {
        font-weight: 400;
      }
      }
    }
  }
  .content4 {
    position: absolute;
    text-align: justify;
    top: 95px;
    left: 180px;
    width: 150px;
    @media (min-width:1440px) {
      top: 130px;
      left: 255px;
      width: 210px;
      text-align: justify;
    }
    @media (min-width: $breakpoint-sm) and (max-width: ($breakpoint-xl - 1px)) {
      top: 95px;
    }

    @media (min-width:$breakpoint-md) and (max-width: ($breakpoint-lg - 1px)) {
      left: 220px; 
      top: 115px;
      }
    .text {
      font-size: 8px;
      line-height: 13px;

      @media (min-width: $breakpoint-sm) and (max-width: ($breakpoint-xl - 1px)) {
        font-size: 6px;
        line-height: 8px;
        width: 135px;
      }

      @media (min-width:$breakpoint-md) and (max-width: ($breakpoint-lg - 1px)) {
        width: 120%;
        font-size: 8.5px;
        line-height: 10px;
      }

      span {
        font-weight: 700;
        @media (min-width: $breakpoint-sm) and (max-width: ($breakpoint-xl - 1px)) {
          font-weight: 400;
        }
      }
    }
  }
  .content5 {
    position: absolute;
    text-align: justify;
    top: 220px;
    left: 180px;
    width: 150px;
    @media (min-width:1440px) {
      top: 320px;
      left: 255px;
      width: 210px;
      text-align: justify;
    }

    @media (min-width:$breakpoint-md) and (max-width: ($breakpoint-lg - 1px)) {
      left: 220px; 
      top: 275px;
      }

    .text {
      font-size: 8px;
      line-height: 15px;

      @media (min-width: $breakpoint-sm) and (max-width: ($breakpoint-xl - 1px)) {
        font-size: 6px;
        line-height: 8px;
        width: 135px;

      }

      @media (min-width:$breakpoint-md) and (max-width: ($breakpoint-lg - 1px)) {
        width: 120%;
        font-size: 8.5px;
        line-height: 10px;
      }

      span {
        font-weight: 700;
        @media (min-width: $breakpoint-sm) and (max-width: ($breakpoint-xl - 1px)) {
          font-weight: 400;
        }
      }
    }
  }
}
</style>

<template>
  <div>
    <div style="display: none">
      <div id="p5t">{{ $t("p5.title") }}</div>
      <div id="p5p1">{{ $t("p5.paragraph1") }}</div>
      <div id="p5p2">{{ $t("p5.paragraph2") }}</div>
      <div id="p5p3">{{ $t("p5.paragraph3") }}</div>
      <div id="p5p4">{{ $t("p5.paragraph4") }}</div>
    </div>
    <div class="content1">
      <div id="p5t_" class="title"></div>
    </div>
    <div class="content2">
      <div id="p5p1_" class="text"></div>
    </div>
    <div class="content3">
      <div id="p5p2_" class="text"></div>
    </div>
    <div class="content4">
      <div id="p5p3_" class="text"></div>
    </div>
    <div class="content5">
      <div id="p5p4_" class="text"></div>
    </div>
  </div>
</template>

<script>
export default {
  name: "Page5",
  mounted() {
    let ref = this;
    ref.processText("p5t");
    ref.processText("p5p1");
    ref.processText("p5p2");
    ref.processText("p5p3");
    ref.processText("p5p4");
    window
      .jQuery("body")
      .on("DOMSubtreeModified", "#p5t, #p5p1, #p5p2,#p5p3,#p5p4", function () {
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