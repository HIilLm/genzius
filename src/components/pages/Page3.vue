<style lang="scss">
.p4 {
  background-image: url("/img/pages/g-03.webp");
  background-position: center;
  background-repeat: no-repeat;
  background-size: cover;
  position: relative;
  /* TEMPLATE 
      // @media (min-width: $breakpoint-xl) { // LAPTOP XL
       
      // }

      // @media (min-width:$breakpoint-lg) and (max-width:($breakpoint-xl - 1px )) { LAPTOP LARGE
        
      // }

      // @media (min-width:$breakpoint-md) and (max-width: ($breakpoint-lg - 1px)) { TABLET
        
      // }
      
      // @media (min-width: $breakpoint-sm) and (max-width: 600px) { HP
        
      // }
  /TEMPLATE*/
  .content1 {
    position: absolute;
    top: 110px;
    left: 20px;

    @media (min-width: 1440px) {
      top: 70px;
      left: 50px;
    }

    @media (min-width: $breakpoint-lg) and (max-width: ($breakpoint-xl - 1px)) {
      top: 50px;
      left: 10px;
    }

    @media (min-width: 481px) and (max-width: ($breakpoint-lg - 1px)) {
      top: 95px;
      left: 10px;
    }

    @media (min-width:$breakpoint-md) and (max-width: ($breakpoint-lg - 1px)) {
      top: 45px;
      left: 15px;
      width: 100%;
    }

    @media (min-width: $breakpoint-sm) and (max-width: 480px) {
      top: 45px;
      left: 13px;
      width: 500px;
    }

    .subtitle {
      span {
        color: #ffffff;
        font-weight: 1000;
        text-align: center;
        margin-left: 20px;
        letter-spacing: 2px;
        font-size: 2rem;

        @media (min-width: $breakpoint-lg) and (max-width: ($breakpoint-xl - 1px)) {
          font-size: 25px;
        }

        @media (min-width: 481px) and (max-width: ($breakpoint-lg - 1px)) {
          font-size: 1.2rem;
        }

        @media (min-width:$breakpoint-md) and (max-width: ($breakpoint-lg - 1px)) {
          font-size: 2rem;
        }

        @media (min-width: $breakpoint-sm) and (max-width: 480px) {
          font-size: 23px;
        }
      }
    }
  }
  .content { 
    position: absolute;
    top: 110px;
    color: #ffffff;
    // left: 20px;
    font-size: 20px;

    @media (min-width: 1440px) {
      top: 110px;
      left: 170px;
    }

    @media (min-width: $breakpoint-lg) and (max-width: ($breakpoint-xl - 1px)) {
      top: 85px;
      left: 120px;
    }

    @media (min-width: 481px) and (max-width: ($breakpoint-lg - 1px)) {
      top: 95px;
      left: 10px;
    }

    @media (min-width:$breakpoint-md) and (max-width: ($breakpoint-lg - 1px)) {
      top: 80px;
      left: 150px;
    }

    @media (min-width: $breakpoint-sm) and (max-width: 480px) {
      top: 75px;
      left: 105px;
    }

    .title {
      span {
        font-weight: 700;
        font-size: 1.7rem;
        letter-spacing: 3px;
        line-height: 1px;

        @media (min-width: $breakpoint-lg) and (max-width: ($breakpoint-xl - 1px)) {
          font-size: 1.1rem;
        }

        @media (min-width: 481px) and (max-width: ($breakpoint-lg - 1px)) {
          font-size: 1.2rem;
        }

        @media (min-width: $breakpoint-sm) and (max-width: 480px) {
          font-size: 1rem;
        }
      }
    }

    .subtitle {
      span {
        color: #ffffff;
        font-weight: 1000;
        text-align: center;
        margin-left: 20px;
        letter-spacing: 2px;
        font-size: 2rem;
        
        @media (min-width: $breakpoint-lg) and (max-width: ($breakpoint-xl - 1px)) {
          font-size: 25px;
        }

        @media (min-width: 481px) and (max-width: ($breakpoint-lg - 1px)) {
          font-size: 1.2rem;
        }

        @media (min-width:$breakpoint-md) and (max-width: ($breakpoint-lg - 1px)) {
          font-size: 2rem;
        }

        @media (min-width: $breakpoint-sm) and (max-width: 480px) {
          font-size: 1rem;
        }
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

    @media (min-width:1440px) {
      top: 155px;
      left: 70px;
      width: 350px;
      font-size: 12px;
      font-weight: 100px;
    }

    @media (min-width: $breakpoint-lg) and (max-width: ($breakpoint-xl - 1px)) {
      top: 130px;
      width: 300px;
      left: 30px;
      font-size: 8.8px;
    }

    @media (min-width: 481px) and (max-width: ($breakpoint-lg - 1px)) {
      top: 202px;
      width: 210px;
      left: 185px;
      font-size: 0.65rem;
    }

    @media (min-width:$breakpoint-md) and (max-width: ($breakpoint-lg - 1px)) {
      top:120px;
      left: 40px;
      width: 80%;
    }

    @media (min-width: $breakpoint-sm) and (max-width: 480px) {
      top: 105px;
      width: 270px;
      left: 30px;
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

      @media (min-width:$breakpoint-md) and (max-width: ($breakpoint-lg - 1px)) {
        line-height: 14px;
      }

      @media (min-width: $breakpoint-sm) and (max-width: 480px) {
        line-height: 11px;
      }
    }

    .text2::first-letter {
      color: #ffffff;
      font-size: 2rem;
      font-weight: 400px;
      float:left;
      line-height: 20px;
      margin-left: 0px;
    }
  }
}
</style>

<template>
  <div>
    <div style="display: none">
      <div id="p3s">{{ $t("p3.subtitle") }}</div>
      <div id="p3p1">{{ $t("p3.paragraph1") }}</div>
      <div id="p3p2">{{ $t("p3.paragraph2") }}</div>
      <div id="p3p3">{{ $t("p3.paragraph3") }}</div>
    </div>
    <div class="content1">
      <div id="p3t_" class="title"></div>
      <div id="p3s_" class="subtitle"></div>
    </div>
    <div class="content">
      <div id="p3p1_" class="text1"></div>
    </div>
    <div class="content2">
      <div id="p3p2_" class="text2"></div>
      <div id="p3p3_" class="text3"></div>
    </div>
  </div>
</template>

<script>
export default {
  name: "Page3",
  mounted() {
    let ref = this;
    ref.processText("p3s");
    ref.processText("p3p1");
    ref.processText("p3p2");
    ref.processText("p3p3");
    window
      .jQuery("body")
      .on("DOMSubtreeModified", "#p3s, #p3p1, #p3p2, #p3p3", function () {
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