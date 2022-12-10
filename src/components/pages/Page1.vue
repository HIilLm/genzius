<style lang="scss">
.p2 {
  background-image: url("/img/pages/g-02.jpg");
  background-position: center;
  background-repeat: no-repeat;
  background-size: cover;
  position: relative;

  .content1{
    color: #ffffff;
    // position: absolute;
    // top: 110px;
    // left: 20px;
    

    // mengatur posisi teks dari atas
    @media (min-width: $breakpoint-lg) and (max-width: ($breakpoint-xl - 1px)) {
      top: 50px;
    }

    @media (min-width: 481px) and (max-width: ($breakpoint-lg - 1px)) {
      top: 215px;
    }

    @media (min-width: $breakpoint-sm) and (max-width: 480px) {
      top: 165px;
    }

    .title {
      // memisahkan title dengan paragraf
      text-align: center;
      margin-bottom: 5px;
      text-align: left;
      margin-left: 10px;
      margin-top: 50px;

      @media (min-width: $breakpoint-sm) and (max-width: 480px) {
        margin-bottom: 0px;
      }

      span {
        font-weight: 700;
        font-size: 3rem;

        @media (min-width: $breakpoint-lg) and (max-width: ($breakpoint-xl - 1px)) {
          font-size: 2rem;
        }

        @media (min-width: 481px) and (max-width: ($breakpoint-lg - 1px)) {
          font-size: 1.6rem;
        }

        @media (min-width: $breakpoint-sm) and (max-width: 480px) {
          margin-bottom: 0px;
          font-size: 1.6rem;
        }
      }
    }

    .text {
      font-size: rem;
      text-align:left;
      line-height: 20px;
      padding-left: 35px;
      padding-right: 10px;

      @media (min-width: $breakpoint-lg) and (max-width: ($breakpoint-xl - 1px)) {
        font-size: 2rem;
        line-height: 10px;
      }

      @media (min-width: 481px) and (max-width: ($breakpoint-lg - 1px)) {
        font-size: 0.7rem;
        line-height: 12px;
      }

      @media (min-width: $breakpoint-sm) and (max-width: 480px) {
        font-size: 0.5rem;
        line-height: 9px;
      }
    }
  }
}
</style>

<template>
  <div>
    
  </div>
</template>

<script>
import jQuery from "jquery";

window.jQuery = jQuery;

export default {
  name: "Page1",
  mounted() {
    let ref = this;
    ref.processText("p1t");
    ref.processText("p1p1");
    window.jQuery("body").on("DOMSubtreeModified", "#p1t, #p1p1", function () {
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
        console.log(id.slice(-1));
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