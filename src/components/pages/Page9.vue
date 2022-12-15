<style lang="scss">
.p10 {
  background-image: url("/img/pages/g-09.webp");
  background-position: center;
  background-repeat: no-repeat;
  background-size: cover;
  position: relative;

  .contentb {
    color: #399876;
    position: absolute;
    top: 20px;
    left: 120px;
    width: 150px;
    @media (min-width:1440px) {
      top: 50px;
      left: 180px;
      width: 450px;
    } 
    @media (min-width: $breakpoint-sm) and (max-width: ($breakpoint-xl - 1px)){
     left: 105px; 
    }
    .title {
      @media (min-width:1440px) {
        font-size: 25px;
        line-height: 12px;
        font-weight: 500;
      } 
      font-size: 2rem;
      line-height: 30px;
      @media (min-width: $breakpoint-sm) and (max-width: ($breakpoint-xl - 1px)) {
        font-size: 20px;
        line-height: 25px;
        width: 500px;
      }
      span {
        font-weight: 700;
      }
    }
  }
  .content1 {
    color: #399876;
    position: absolute;
    top: 40px;
    left: 105px;
    width: 150px;
    @media (min-width:1440px) {
      top: 75px;
      left: 150px;
      width: 250px;
      text-align: center;
    } 
    @media (min-width: $breakpoint-sm) and (max-width: ($breakpoint-xl - 1px)){
     left: 95px; 
    }
    .title {
      @media (min-width:1440px) {
        font-size: 30px;
        line-height: 12px;
        font-weight: 500;
      } 
      font-size: 2rem;
      line-height: 30px;

      @media (min-width: $breakpoint-sm) and (max-width: ($breakpoint-xl - 1px)) {
        font-size: 20px;
        line-height: 25px;
        width: 170px;
        text-align: center;
      }

      span {
        font-weight: 800;
      }
    }
  }
  .content2 {
    ::first-letter{
      color: #399876;
      font-size: 2rem;
      font-weight: 700;
      float:left;
      line-height: 10px;
      margin-left: 0px;
    }
    @media (min-width:1440px) {
      top: 100px;
      left: 50px;
      width: 400px;
    } 
    color: #399876;
    position: absolute;
    text-align: justify;
    top: 80px;
    left: 20px;
    width: 150px;

    @media (min-width: $breakpoint-sm) and (max-width: ($breakpoint-xl - 1px)){
     left: 20px;
     top: 65px;
    }

    .text {
      @media (min-width:1440px) {
        font-size: 10px;
        line-height: 12px;
        font-weight: 500;
      } 
      font-size: 2rem;
      line-height: 30px;

      @media (min-width: $breakpoint-sm) and (max-width: ($breakpoint-xl - 1px)) {
        font-size: 7px;
        line-height: 9px;
        width: 300px;
      }

      span {
        font-weight: 600;
      }
    }
  }
  .content3 {
    color: #399876;
    position: absolute;
    text-align: justify;
    top: 140px;
    left: 20px;
    width: 150px;
    @media (min-width:1440px) {
      top: 190px;
      left: 50px;
      width: 400px;
    } 

    @media (min-width: $breakpoint-sm) and (max-width: ($breakpoint-xl - 1px)){
     top: 128px; 
    }

    .text {
      @media (min-width:1440px) {
        font-size: 10px;
        line-height: 12px;
        font-weight: 500;
      } 
      font-size: 2rem;
      line-height: 30px;

      @media (min-width: $breakpoint-sm) and (max-width: ($breakpoint-xl - 1px)) {
        font-size: 7px;
        line-height: 10px;
        width: 300px;
      }

      span {
        font-weight: 600;
      }
    }
  }
  .content4 {
    color: #399876;
    position: absolute;
    text-align: justify;
    top: 215px;
    left: 20px;
    width: 150px;
    @media (min-width:1440px) {
      top: 295px;
      left: 50px;
      width: 400px;
    } 
    @media (min-width: $breakpoint-sm) and (max-width: ($breakpoint-xl - 1px)){
     top: 199px; 
    }
    .text {
      @media (min-width:1440px) {
        font-size: 10px;
        line-height: 12px;
        font-weight: 500;
      } 
      font-size: 2rem;
      line-height: 30px;

      @media (min-width: $breakpoint-sm) and (max-width: ($breakpoint-xl - 1px)) {
        font-size: 7px;
        line-height: 10px;
        width: 300px;
      }

      span {
        font-weight: 600;
      }
    }
  }
}
</style>

<template>
  <div>
    <div style="display: none">
      <div id="p9t">{{ $t("p9.title") }}</div>
      <div id="p9p1">{{ $t("p9.paragraph1") }}</div>
      <div id="p9p2">{{ $t("p9.paragraph2") }}</div>
      <div id="p9p3">{{ $t("p9.paragraph3") }}</div>
      <div id="p9p4">{{ $t("p9.paragraph4") }}</div>
    </div>

    <div class="contentb">
      <div id="p9t_" class="title"></div>
    </div>
    <div class="content1">
      <div id="p9p1_" class="title"></div>
    </div>
    <div class="content2">
      <div id="p9p2_" class="text"></div>     
    </div>
    <div class="content3">
      <div id="p9p3_" class="text"></div>      
    </div>
    <div class="content4">
      <div id="p9p4_" class="text"></div>
    </div>
  </div>
</template>

<script>
export default {
  name: "Page9",
  mounted() {
    let ref = this;
    ref.processText("p9t");
    ref.processText("p9p1");
    ref.processText("p9p2");
    ref.processText("p9p3");
    ref.processText("p9p4");
    window
      .jQuery("body")
      .on(
        "DOMSubtreeModified",
        "#p9t, #p9p1, #p9p2, #p9p3, #p9p4",
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
  },
};
</script>