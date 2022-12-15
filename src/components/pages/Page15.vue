<style lang="scss" scoped>
.p16 {
  background-image: url("/img/pages/g-15.webp");
  background-position: center;
  background-repeat: no-repeat;
  background-size: cover;
  position: relative;

  .content1 {
    color: #fff;
    position: absolute;
    text-align: center;
    top: 350px;
    left: 50px;
    width: 150px;
    @media (min-width: 1440px) {
     top: 480px;
     left:100px;
    }
    @media (min-width: $breakpoint-sm) and (max-width: ($breakpoint-xl - 1px)){
     top: 320px;
     left: 25px;
    }

    .text {
      font-size: 2rem;
      line-height: 30px;
      @media (min-width: $breakpoint-sm) and (max-width: ($breakpoint-xl - 1px)) {
        font-size: 10.5px;
        line-height: 10px;
        width: 290px;
      }

      @media (min-width: 1440px) {
        font-size: 12px;
        line-height: 11px;
        width: 290px;
      }

      span {
        font-weight: 700;
      }
    }
  }

  .content2 {
    color: #fff;
    position: absolute;
    text-align: center;
    top: 280px;
    left: 50px;
    width: 150px;
    @media (min-width: 1440px) {
     top: 380px;
     left:100px;
    }
    @media (min-width: $breakpoint-sm) and (max-width: ($breakpoint-xl - 1px)){
     top: 256px;
     left: 25px;
    }

    .text {
      font-size: 2rem;
      line-height: 30px;

      @media (min-width: $breakpoint-sm) and (max-width: ($breakpoint-xl - 1px)) {
        font-size: 10.5px;
        line-height: 10px;
        width: 290px;

      }
      @media (min-width: 1440px) {
        font-size: 12px;
        line-height: 11px;
        width: 290px;
      }

      span {
        font-weight: 700;
      }
    }
  }
  .content3 {
    color: #fff;
    position: absolute;
    text-align: center;
    top: 210px;
    left: 50px;
    width: 150px;
    @media (min-width: 1440px) {
     top: 280px;
     left:100px;
    }
    @media (min-width: $breakpoint-sm) and (max-width: ($breakpoint-xl - 1px)){
     top: 185px; 
     left: 25px;
    }

    .text {
      font-size: 2rem;
      line-height: 30px;
      @media (min-width: $breakpoint-sm) and (max-width: ($breakpoint-xl - 1px)) {
        font-size: 10.5px;
        line-height: 10px;
        width: 290px;
      }

      @media (min-width: 1440px) {
        font-size: 12px;
        line-height: 11px;
        width: 290px;
      }

      span {
        font-weight: 700;
      }
    }
  }
  .content4 {
    color: #fff;
    position: absolute;
    text-align: center;
    top: 160px;
    left: 50px;
    width: 150px;
    @media (min-width: 1440px) {
      top: 215px;
      left: 100px;
    }
    @media (min-width: $breakpoint-sm) and (max-width: ($breakpoint-xl - 1px)){
     top: 140px; 
     left: 25px;
    }
    .text {
      font-size: 2rem;
      line-height: 30px;

      @media (min-width: $breakpoint-sm) and (max-width: ($breakpoint-xl - 1px)) {
        font-size: 10.5px;
        line-height: 11px;
        width: 290px;
      }

      @media (min-width: 1440px) {
        font-size: 12px;
        line-height: 11px;
        width: 290px;
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
      <div id="p15t">{{ $t("p15.title") }}</div>
      <div id="p15p1">{{ $t("p15.paragraph1") }}</div>
      <div id="p15p2">{{ $t("p15.paragraph2") }}</div>
      <div id="p15p3">{{ $t("p15.paragraph3") }}</div>
      <div id="p15p4">{{ $t("p15.paragraph4") }}</div>
    </div>

    <div class="content4">
      <div id="p15t_" class="text"></div>
      <div id="p15p1_" class="text"></div>
    </div>
    <div class="content3">
      <div id="p15p2_" class="text"></div>
    </div>
    <div class="content2">
      <div id="p15p3_" class="text"></div>
    </div>
    <div class="content1">
      <div id="p15p4_" class="text"></div>
    </div>
  </div>
</template>

<script>
export default {
  name: "Page15",
  mounted() {
    let ref = this;
    ref.processText("p15t");
    ref.processText("p15p1");
    ref.processText("p15p2");
    ref.processText("p15p3");
    ref.processText("p15p4");
    window
      .jQuery("body")
      .on("DOMSubtreeModified", "#p15t,#p15p1,#p15p2,#p15p3,#p15p4", function () {
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