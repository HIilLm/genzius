<style lang="scss">
.p7 {
  background-image: url("/img/pages/g-06.jpg");
  background-position: center;
  background-repeat: no-repeat;
  background-size: cover;
  position: relative;

  .content {
    position: absolute;
    color:orangered;
    top: 53px;
    font-size: 0.7rem;
    font-weight: bold;

    @media (min-width: $breakpoint-lg) and (max-width: ($breakpoint-xl - 1px)) {
      font-size: 23px;
      top: 140px;
      left: 30px;
      line-height: 10px;
    }

    @media (min-width: 481px) and (max-width: ($breakpoint-lg - 1px)) {
      font-size: 0.65rem;
      top: 45px;
      line-height: 11px;
    }

    @media (min-width: $breakpoint-sm) and (max-width: 480px) {
      font-size: 0.5rem;
      top: 35px;
      line-height: 10px;
    }

  }
  .content2 {
    ::first-letter{
      color: #ffffff;
      font-size: 2rem;
      font-weight: 600;
      float:left;
      line-height: 20px;
      margin-left: 0px;
    }
    position: absolute;
    top: 53px;
    grid-template-columns: 50% 50%;
    font-size: 0.7rem;

    @media (min-width: $breakpoint-lg) and (max-width: ($breakpoint-xl - 1px)) {
      color: white;
      font-size: 9px;
      font-weight: 300;
      width: 310px;
      top: 30px;
      left: -5px;
      line-height: 10px;
    }

    @media (min-width: 481px) and (max-width: ($breakpoint-lg - 1px)) {
      font-size: 0.65rem;
      top: 45px;
      line-height: 11px;
    }

    @media (min-width: $breakpoint-sm) and (max-width: 480px) {
      font-size: 0.5rem;
      top: 35px;
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
    </div>
    <div class="content">
      <div class="">
        <div id="p6p1_" class="text1"></div>
      </div>
      <div class="content2">
        <div id="p6p2_" class="text"></div>
      </div>
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
    window.jQuery("body").on("DOMSubtreeModified", "#p6p1, #p6p2", function () {
      ref.processText(window.jQuery(this).attr("id"));
    });
  },
  methods: {
    processText(id) {
      let text = document.getElementById(id).textContent;
      let r = text.split(".");
      document.getElementById(id + "_").innerHTML = "";
      window.jQuery.each(r, function (i, w) {
        var node = document.createElement("span");
        var textnode = document.createTextNode(
          w + (id.slice(-1) == "t" || id.slice(-1) == "s" ? "" : ".")
        );
        node.appendChild(textnode);
        document.getElementById(id + "_").appendChild(node);
      });
    },
  },
};
</script>