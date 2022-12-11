<style lang="scss">
.p15 {
  background-image: url("/img/pages/g-14.jpg");
  background-position: center;
  background-repeat: no-repeat;
  background-size: cover;
  position: relative;

  .content {
    // color: #ffffff;
    position: absolute;
    top: 20px;
    left: 130px;
    width: 150px;
    .title {
      font-size: 2rem;
      line-height: 30px;

      @media (min-width: $breakpoint-sm) and (max-width: ($breakpoint-xl - 1px)) {
        font-size: 20px;
        line-height: 25px;
        width: 500px;
      }

      span {
        font-weight: 500;
      }
    }
  }
  .content1 {
    // color: #ffffff;
    position: absolute;
    top: 40px;
    left: 125px;
    width: 150px;
    .title {
      font-size: 2rem;
      line-height: 30px;

      @media (min-width: $breakpoint-sm) and (max-width: ($breakpoint-xl - 1px)) {
        font-size: 30px;
        line-height: 25px;
        width: 500px;
      }

      span {
        font-weight: 800;
      }
    }
  }
  .content2 {
    color: orangered;
    position: absolute;
    top: 80px;
    left: 90px;
    width: 150px;
    .title {
      font-size: 2rem;
      line-height: 30px;

      @media (min-width: $breakpoint-sm) and (max-width: ($breakpoint-xl - 1px)) {
        font-size: 13px;
        line-height: 25px;
        width: 500px;
      }

      span {
        font-weight: 800;
      }
    }
  }
  .content3 {
    position: absolute;
    text-align: justify;
    top: 100px;
    left: 90px;
    width: 150px;

    .text {
      font-size: 2rem;
      line-height: 30px;

      @media (min-width: $breakpoint-sm) and (max-width: ($breakpoint-xl - 1px)) {
        font-size: 7.8px;
        line-height: 10px;
        width: 235px;

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
      <div id="p14t">{{ $t("p14.title") }}</div>
      <div id="p14t2">{{ $t("p14.title2") }}</div>
      <div id="p14t3">{{ $t("p14.title3") }}</div>
      <div id="p14p1">{{ $t("p14.paragraph1") }}</div>
      <div id="p14p2">{{ $t("p14.paragraph2") }}</div>
      <div id="p14p3">{{ $t("p14.paragraph3") }}</div>
      <div id="p14p4">{{ $t("p14.paragraph4") }}</div>
      <div id="p14p5">{{ $t("p14.paragraph5") }}</div>
    </div>

    <div class="content">
      <div id="p14t_" class="title"></div>
    </div>
    <div class="content1">
      <div id="p14t2_" class="title"></div>
    </div>
    <div class="content2">
      <div id="p14t3_" class="title"></div>
    </div>
    <div class="content3">
      <div id="p14p1_" class="text"></div>
    </div>
  </div>
</template>

<script>
export default {
  name: "Page14",
  mounted() {
    let ref = this;
    ref.processText("p14t");
    ref.processText("p14t2");
    ref.processText("p14t3");
    ref.processText("p14p1");
    ref.processText("p14p2");
    ref.processText("p14p3");
    ref.processText("p14p4");
    ref.processText("p14p5");
    window
      .jQuery("body")
      .on(
        "DOMSubtreeModified",
        "#p14t,#p14t2,#p14t3,#p14p1,#p14p2,#p14p3,#p14p4,#p14p5",
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