<style lang="scss">
.p7 {
  background-image: url("/img/pages/g-06.webp");
  background-position: center;
  background-repeat: no-repeat;
  background-size: cover;
  position: relative;
  // TEMPLATE 
  // @media (min-width: $breakpoint-xl) { // LAPTOP XL

  // }

  // @media (min-width:$breakpoint-lg) and (max-width:($breakpoint-xl - 1px )) { LAPTOP LARGE

  // }

  // @media (min-width:$breakpoint-md) and (max-width: ($breakpoint-lg - 1px)) { // TABLET

  // }

  // @media (min-width: $breakpoint-sm) and (max-width: 480px) { HP

  // }
  //TEMPLATE
  .contentq {
    position: absolute;
    color: #ffffff;
    top: 53px;
    font-weight: 900;
    text-align: justify;

    @media (min-width: $breakpoint-xl) {
      // LAPTOP XL
      top: 190px;
      left: 90px;
      width: 350px;
      font-size: 22px;
    }

    @media (min-width: $breakpoint-lg) and (max-width: ($breakpoint-xl - 1px)) {
      font-size: 21px;
      top: 140px;
      left: 25px;
      line-height: 10px;
    }

    @media (min-width:$breakpoint-md) and (max-width: ($breakpoint-lg - 1px)) {
      // TABLET
      top: 165px;
      left: 79px;
      font-size: 19px;
    }

    @media (min-width: $breakpoint-sm) and (max-width: 480px) {
      font-size: 18px;
      top: 130px;
      left: 40px;
      line-height: 10px;
    }

  }

  .content2 {
    ::first-letter {
      color: orangered;
      font-size: 2rem;
      font-weight: 500;
      float: left;
      line-height: 25px;
    }

    position: absolute;
    text-align: justify;
    color: orangered;

    @media (min-width: $breakpoint-xl) {
      // LAPTOP XL

      top: 250px;
      left: 30px;
      width: 430px;
      font-size: 11px;

    }

    @media (min-width: $breakpoint-lg) and (max-width: ($breakpoint-xl - 1px)) {

      font-size: 9px;
      font-weight: 300;
      width: 300px;
      top: 40px;
      left: 0px;
      line-height: 10px;
    }

    @media (min-width:$breakpoint-md) and (max-width: ($breakpoint-lg - 1px)) {
      // TABLET

      top: 220px;
      left: 30px;
      width: 363px;
      font-size: 9px;
    }

    @media (min-width: $breakpoint-sm) and (max-width: ($breakpoint-md - 1px)) {

      font-size: 8px;
      font-weight: 300;
      width: 310px;
      top: 160px;
      left: 20px;
      line-height: 10px;
      text-align: justify;
      width: 287px;
    }

  }

  .content3 {
    position: absolute;
    top: 53px;
    text-align: justify;
    color: orangered;

    @media (min-width: $breakpoint-xl) {
      // LAPTOP XL
      top: 330px;
      left: 30px;
      font-size: 11px;
      width: 430px;

    }

    @media (min-width: $breakpoint-lg) and (max-width: ($breakpoint-xl - 1px)) {
      font-size: 9px;
      font-weight: 300;
      width: 300px;
      top: 95px;
      left: 0px;
      line-height: 10px;
    }

    @media (min-width:$breakpoint-md) and (max-width: ($breakpoint-lg - 1px)) {
      // TABLET
      top: 290px;
      left: 30px;
      font-size: 9px;
      width: 363px;
    }

    @media (min-width: $breakpoint-sm) and (max-width: 480px) {

      font-size: 8px;
      font-weight: 300;
      width: 285px;
      top: 220px;
      left: 20px;

      line-height: 10px;
    }

  }

  .content4 {
    position: absolute;
    top: 53px;
    grid-template-columns: 50% 50%;
    font-size: 0.7rem;
    color: orangered;
    text-align: justify;

    @media (min-width: $breakpoint-xl) {
      // LAPTOP XL
      top: 470px;
      left: 30px;
      font-size: 11px;
      width: 430px;

    }

    @media (min-width: $breakpoint-lg) and (max-width: ($breakpoint-xl - 1px)) {
      font-size: 9px;
      font-weight: 300;
      width: 300px;
      top: 190px;
      left: 0px;
      line-height: 10px;
    }

    @media (min-width:$breakpoint-md) and (max-width: ($breakpoint-lg - 1px)) {
      // TABLET
      top: 410px;
      left: 30px;
      font-size: 9px;
      width: 363px;
    }

    @media (min-width: $breakpoint-sm) and (max-width: 480px) {
      font-size: 8px;
      font-weight: 300;
      width: 285px;
      top: 320px;
      left: 20px;
      line-height: 10px;
    }

  }
}
</style>

<template>
  <div>
    <div style="display: none">
      <div id="p6p1">{{ $t("p6.paragraph1") }}</div>
      <div id="p6p2">{{ $t("p6.paragraph2") }}</div>
      <div id="p6p3">{{ $t("p6.paragraph3") }}</div>
      <div id="p6p4">{{ $t("p6.paragraph4") }}</div>
    </div>
    <div class="contentq">
      <div id="p6p1_" class="text1"></div>
    </div>
    <div class="content2">
      <div id="p6p2_" class="text"></div>
    </div>
    <div class="content3">
      <div id="p6p3_" class="text"></div>
    </div>
     <div class="content4">
        <div id="p6p4_" class="text"></div>
      </div>
  </div>
</template>

<script>
export default {
  name: "Page6",
  mounted() {
    let ref = this;
    ref.processText("p6p1");
    ref.processText("p6p2");
    ref.processText("p6p3");
    ref.processText("p6p4");
    window.jQuery("body").on("DOMSubtreeModified", "#p6p1, #p6p2, #p6p3, #p6p4", function () {
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