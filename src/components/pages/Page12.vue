<style lang="scss">
.p13 {
  background-image: url("/img/pages/12.jpg");
  background-position: center;
  background-repeat: no-repeat;
  background-size: cover;
  position: relative;

  .content {
    color: #793c84;
    position: absolute;
    top: 15px;
    left: 80px;
    width: 140px;
    padding-left: 15px;
    @media (min-width:1440px) {
      left: 115px;
      top: 30px; 
      width: 200px;
    } 
    .title {
      font-size: 2rem;
      line-height: 30px;
      @media (min-width:1440px) {
        font-size: 28px;
        width: 800px;
      }  
      @media (min-width: $breakpoint-sm) and (max-width: ($breakpoint-xl - 1px)) {
        font-size: 20px;
        line-height: 25px;
        width: 400px;
      }

      span {
        font-weight: 500;
      }
    }
  }
  .content1 {
    color: #766daf;
    position: absolute;
    top: 40px;
    left: 65px;
    padding-left: 15px;
    width: 140px;
    @media (min-width:1440px) {
      left: 110px;
      top: 65px; 
      width: 200px;
    } 
    .title {
      font-size: 2rem;
      line-height: 30px;
      @media (min-width:1440px) {
        font-size: 28px;
        width: 800px;
      }   
      @media (min-width: $breakpoint-sm) and (max-width: ($breakpoint-xl - 1px)) {
        font-size: 23px;
        line-height: 25px;
        width: 400px;
      }

      span {
        font-weight: 800;
      }
    }
  }
  .content2 {
    position: absolute;
    text-align: justify;
    top: 80px;
    left: 10px;
    width: 150px;
    @media (min-width:1440px) {
      left: 30px;
      top: 110px; 
      width: 180px;
    } 
    @media (min-width: $breakpoint-sm) and (max-width: ($breakpoint-xl - 1px)){
        top: 80px;
    }
    .text {
      @media (min-width:1440px) {
        font-size: 10px;
        width: 440px;
        line-height: 13px;
      }  
      font-size: 2rem;
      line-height: 30px;

      @media (min-width: $breakpoint-sm) and (max-width: ($breakpoint-xl - 1px)) {
        font-size: 7.8px;
        line-height: 8px;
        width: 313px;
      }

      span {
        font-weight: 500;
      }
    }
  }
  .content3 {
    position: absolute;
    text-align: justify;
    top: 135px;
    left: 10px;
    width: 150px;
    @media (min-width:1440px) {
      left: 30px;
      top: 190px; 
      width: 180px;
    } 
    @media (min-width: $breakpoint-sm) and (max-width: ($breakpoint-xl - 1px)){
        top: 126px;
    }
    .text {
      @media (min-width:1440px) {
        font-size: 10px;
        width: 440px;
        line-height: 13px;
      }  
      font-size: 2rem;
      line-height: 30px;

      @media (min-width: $breakpoint-sm) and (max-width: ($breakpoint-xl - 1px)) {
        font-size: 7.8px;
        line-height: 9px;
        width: 313px;

      }

      span {
        font-weight: 500;
      }
    }
  }
  .content4 {
    position: absolute;
    text-align: justify;
    top: 200px;
    left: 10px;
    width: 150px;
    @media (min-width:1440px) {
      left: 30px;
      top: 280px; 
      width: 180px;
    } 
    @media (min-width: $breakpoint-sm) and (max-width: ($breakpoint-xl - 1px)){
      top: 187px;
    }
    .text {
      @media (min-width:1440px) {
        font-size: 10px;
        width: 440px;
        line-height: 13px;
      }  
      font-size: 2rem;
      line-height: 30px;

      @media (min-width: $breakpoint-sm) and (max-width: ($breakpoint-xl - 1px)) {
        font-size: 7.8px;
        line-height: 9px;
        width: 313px;
      }

      span {
        font-weight: 500;
      }
    }
  }
  .content5 {
    position: absolute;
    text-align: justify;
    top: 260px;
    left: 10px;
    width: 150px;
    @media (min-width:1440px) {
      left: 30px;
      top: 370px; 
      width: 180px;
    } 
    @media (min-width: $breakpoint-sm) and (max-width: ($breakpoint-xl - 1px)){
      top: 248px;
    }
    .text {
      @media (min-width:1440px) {
        font-size: 10px;
        width: 440px;
        line-height: 13px;
      }  
      font-size: 2rem;
      line-height: 30px;

      @media (min-width: $breakpoint-sm) and (max-width: ($breakpoint-xl - 1px)) {
        font-size: 7.8px;
        line-height: 9px;
        width: 313px;

      }

      span {
        font-weight: 500;
      }
    }
  }
}
</style>

<template>
  <div>
    <div style="display: none">
      <div id="p12pt">{{ $t("p12.title") }}</div>
      <div id="p12p1t">{{ $t("p12.paragraph1t") }}</div>
      <div id="p12p1">{{ $t("p12.paragraph1") }}</div>
      <div id="p12p2t">{{ $t("p12.paragraph2t") }}</div>
      <div id="p12p2">{{ $t("p12.paragraph2") }}</div>
      <div id="p12p3t">{{ $t("p12.paragraph3t") }}</div>
      <div id="p12p3">{{ $t("p12.paragraph3") }}</div>
    </div>

    <div class="content">
      <div id="p12pt_" class="title"></div>
    </div>
    <div class="content1">
      <div id="p12p1t_" class="title"></div>
    </div>
    <div class="content2">
      <div id="p12p1_" class="text"></div>
    </div>
    <div class="content3">
      <div id="p12p2t_" class="text"></div>
    </div>
    <div class="content4">
      <div id="p12p2_" class="text"></div>
    </div>
    <div class="content5">
      <div id="p12p3t_" class="text"></div>
      <div id="p12p3_" class="text"></div>
    </div>
  </div>
</template>

<script>
export default {
  name: "Page12",
  mounted() {
    let ref = this;
    ref.processText("p12pt");
    ref.processText("p12p1t");
    ref.processText("p12p1");
    ref.processText("p12p2t");
    ref.processText("p12p2");
    ref.processText("p12p3t");
    ref.processText("p12p3");
    window
      .jQuery("body")
      .on(
        "DOMSubtreeModified",
        "#p12pt,#p12p1t,#p12p1,#p12p2t,#p12p2,#p12p3t,#p12p3",
        function () {
          ref.processText(window.jQuery(this).attr("id"));
        }
      );
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
    showImage(url) {
      this.$parent.showImage(url);
    },
  },
};
</script>