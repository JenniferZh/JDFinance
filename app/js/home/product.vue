<template lang="html">
  <Panel title="新品推荐" :class="$style.panel">
    <section :class="$style.content">
      <div class="arrow">更多尖货</div>
      <Slider cname="product-slider" :items="items" :options="options"></Slider>
    </section>
  </Panel>
</template>

<script>
import Slider from "../core/slider"
import Panel from "../core/panel"
export default {
  components: {
    Panel,
    Slider,
  },
  data() {
    return {
      items: [
        {
          href:'home',
          src:'//img12.360buyimg.com/jrpmobile/jfs/t19063/263/1067257870/16513/d7360e92/5ab85da9N8af17d57.jpg?width=335&height=421'
        },
        {
          href:'home',
          src:'//img12.360buyimg.com/jrpmobile/jfs/t12637/325/2370404484/14164/523e69a7/5ab85dd5Ndaf12da2.jpg?width=335&height=421'
        },
        {
          href:'home',
          src:'//img12.360buyimg.com/jrpmobile/jfs/t17317/55/1066024964/35575/444c5252/5ab85ddeNaa593024.jpg?width=335&height=421'
        },
        {
          href:'home',
          src:'//img12.360buyimg.com/jrpmobile/jfs/t16600/39/1049384083/42815/1727a973/5ab85debN56037cfc.jpg?width=335&height=421'
        }

      ],
      options: {
          slidesPerView: 2.3,
          spaceBetween: 30,
      }
    }
  }
}
</script>

<style lang="scss" module>
  @import "../../css/element.scss";
  .panel {
    @include panel;
    .content {
      padding-bottom: 40px;
      position: relative;
      &>div {
        font-size: 28px;
        color:#999;
        position:absolute;
        right:20px;
        top:-70px;
      }
    }
  }
</style>

<style lang="scss">
  .product-slider {
    .swiper-container {
      box-sizing: border-box;
      padding: 0 24px;
      .swiper-slide {
        a {
          display: inline-block;
          width: 100%;
          img {
            width: 100%;
            display: block;
            height: 314;
            border: 1px solid red;
          }
        }
      }
    }
  }

</style>
