<template lang="html">
  <article class="">
    <Slider :cname="$style.slider" :items="items"/>
  </article>
</template>

<script>
import Slider from "../core/slider"
export default {
  components: {
    Slider,
  },
  data() {
    return {
      items: [
        {
          href:'home',
          src:'//img12.360buyimg.com/jrpmobile/jfs/t17461/358/1340151638/22046/3f694934/5ac48151Nfb7c9457.jpg?width=750&height=320',
        },
        {
          href:'home',
          src:'//img12.360buyimg.com/jrpmobile/jfs/t17587/360/1294779268/27619/bbe75751/5ac48106N235aa3bb.png?width=750&height=320',
        },
        {
          href:'home',
          src:'//img12.360buyimg.com/jrpmobile/jfs/t16735/202/1316283826/42649/4637640a/5ac4817fN20143151.jpg?width=750&height=320'
        },
      ],

    }
  }
}
</script>

<style lang="scss" module>
  @import "../../css/element.scss";
  .slider {
    margin-top: 120px;
    img {
      width: 100%;
    }
  }


</style>
