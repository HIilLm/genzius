<style lang="scss">
.p12 {
  background-image: url("/img/pages/11.jpg");
  background-position: center;
  background-repeat: no-repeat;
  background-size: cover;
  position: relative;

  .content {
    color: #fff;
    position: absolute;
    top: 15px;
    left: 100px;
    width: 140px;
    padding-left: 15px;
    background-color: #876bfe;
    .title {
      font-size: 2rem;
      line-height: 30px;

      @media (min-width: $breakpoint-sm) and (max-width: ($breakpoint-xl - 1px)) {
        font-size: 20px;
        line-height: 25px;
        width: 400px;
      }

      span {
        font-weight: 600;
      }
    }
  }
  .content1 {
    color: #fff;
    position: absolute;
    top: 45px;
    left: 130px;
    padding-left: 15px;
    background-color: #876bfe;
    width: 140px;
    .title {
      font-size: 2rem;
      line-height: 30px;

      @media (min-width: $breakpoint-sm) and (max-width: ($breakpoint-xl - 1px)) {
        font-size: 20px;
        line-height: 25px;
        width: 400px;
      }

      span {
        font-weight: 800;
      }
    }
  }
  .content2 {
    ::first-letter{
      color: #903e95;
      font-size: 2rem;
      font-weight: 600;
      float:left;
      line-height: 20px;
      margin-left: 0px;
    }
    color: #903e95;
    position: absolute;
    text-align: justify;
    top: 80px;
    left: 10px;
    width: 150px;
    @media (min-width: $breakpoint-sm) and (max-width: ($breakpoint-xl - 1px)){
          top: 75px;
        }
    .text {
      font-size: 2rem;
      line-height: 30px;

      @media (min-width: $breakpoint-sm) and (max-width: ($breakpoint-xl - 1px)) {
        font-size: 6px;
        line-height: 10px;
        width: 312px;
      }

      span {
        font-weight: 700;
        @media (min-width: $breakpoint-sm) and (max-width: ($breakpoint-xl - 1px)){
          font-weight: 600;
        }
      }
    }
  }
  .content3 {
    color: #903e95;
    position: absolute;
    text-align: justify;
    top: 150px;
    left: 10px;
    width: 150px;
    @media (min-width: $breakpoint-sm) and (max-width: ($breakpoint-xl - 1px)){
          top: 145px;
    }
    .text {
      font-size: 2rem;
      line-height: 30px;

      @media (min-width: $breakpoint-sm) and (max-width: ($breakpoint-xl - 1px)) {
        font-size: 6px;
        line-height: 10px;
        width: 312px;
      }

      span {
        font-weight: 700;
        @media (min-width: $breakpoint-sm) and (max-width: ($breakpoint-xl - 1px)){
          font-weight: 600;
        }
      }
    }
  }
  .content4 {
    color: #903e95;
    position: absolute;
    text-align: justify;
    top: 180px;
    left: 10px;
    width: 150px;
    @media (min-width: $breakpoint-sm) and (max-width: ($breakpoint-xl - 1px)){
          top: 175px;
    }
    .text {
      font-size: 2rem;
      line-height: 30px;

      @media (min-width: $breakpoint-sm) and (max-width: ($breakpoint-xl - 1px)) {
        font-size: 6px;
        line-height: 9px;
        width: 312px;
      }

      span {
        font-weight: 700;
        @media (min-width: $breakpoint-sm) and (max-width: ($breakpoint-xl - 1px)){
          font-weight: 600;
        }
      }
    }
  }
  .content5 {
    color: #903e95;
    position: absolute;
    text-align: justify;
    top: 340px;
    left: 10px;
    width: 150px;
    @media (min-width: $breakpoint-sm) and (max-width: ($breakpoint-xl - 1px)){
          top: 322px;
    }
    .text {
      font-size: 2rem;
      line-height: 30px;

      @media (min-width: $breakpoint-sm) and (max-width: ($breakpoint-xl - 1px)) {
        font-size: 6px;
        line-height: 10px;
        width: 312px;
      }

      span {
        font-weight: 700;
        @media (min-width: $breakpoint-sm) and (max-width: ($breakpoint-xl - 1px)){
          font-weight: 600;
        }
      }
    }
  }
  .content6 {
    color: #903e95;
    position: absolute;
    text-align: justify;
    top: 410px;
    left: 10px;
    width: 150px;
    @media (min-width: $breakpoint-sm) and (max-width: ($breakpoint-xl - 1px)){
          top: 394px;
    }
    .text {
      font-size: 2rem;
      line-height: 30px;

      @media (min-width: $breakpoint-sm) and (max-width: ($breakpoint-xl - 1px)) {
        font-size: 6px;
        line-height: 10px;
        width: 280px;
      }
      span {
        font-weight: 700;
        @media (min-width: $breakpoint-sm) and (max-width: ($breakpoint-xl - 1px)){
          font-weight: 600;
        }
      }
    }
}
}
</style>

<template>
  <div>
    <div style="display: none">  
      <div id="p11pt">{{ $t("p11.title") }}</div>
      <div id="p11p1t">{{ $t("p11.paragraph1t") }}</div>
      <div id="p11p1">{{ $t("p11.paragraph1") }}</div>
      <div id="p11p2t">{{ $t("p11.paragraph2t") }}</div>
      <div id="p11p2">{{ $t("p11.paragraph2") }}</div>
      <div id="p11p3t">{{ $t("p11.paragraph3t") }}</div>
      <div id="p11p3">{{ $t("p11.paragraph3") }}</div>
    </div> 

    <div class="content">
      <div id="p11pt_" class="title"></div>
    </div>
    <div class="content1">
      <div id="p11p1t_" class="title"></div>
    </div>
    <div class="content2">
      <div id="p11p1_" class="text"></div>
    </div>
    <div class="content3">
      <div id="p11p2t_" class="text"></div>
    </div>
    <div class="content4">
      <div id="p11p2_" class="text"></div>
    </div>
    <div class="content5">
      <div id="p11p3t_" class="text"></div>
    </div>
    <div class="content6">
      <div id="p11p3_" class="text"></div>
    </div>
  </div>
</template>

<script>
export default {
  name: "Page11",
  mounted() {
    let ref = this;
    ref.processText("p11pt");
    ref.processText("p11p1t");
    ref.processText("p11p1");
    ref.processText("p11p2t");
    ref.processText("p11p2");
    ref.processText("p11p3t");
    ref.processText("p11p3");
    window
      .jQuery("body")
      .on(
        "DOMSubtreeModified",
        "#p11pt,#p11p1t,#p11p1,#p11p2t,#p11p2,#p11p3t,#p11p3",
        function () {
          ref.processText(window.jQuery(this).attr("id"));
        }
      );
  },
  methods: {
    processText(id) {
      let text = document.getElementById(id).textContent;
      let r = text.split("-");
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