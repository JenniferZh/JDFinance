<template lang="html">
  <Panel :class="panel" title="保险保障">
    <Slider cname="inslider" :options="options" :items="items"></Slider>
    <div :class="$style.car">
      <img src="//img12.360buyimg.com/jrpmobile/jfs/t15583/348/2209539372/42536/6bae28a8/5a953b19Nd7e46726.jpg?width=750&height=200" alt="">
    </div>
  </Panel>
</template>

<script>
import Slider from "../core/slider.vue"
import Panel from "../core/panel.vue"
export default {
  components:{
    Slider,
    Panel,
  },
  data() {
    return {
      items: [{
        src:'//img12.360buyimg.com/jrpmobile/jfs/t12355/171/849656870/29064/92c9bc12/5a153643N04efba6e.jpg?width=210&height=260',
        href:'home',
      },{
        src:'//img12.360buyimg.com/jrpmobile/jfs/t10360/347/311063647/10881/14a5cd40/59cb632fNcac82571.jpg?width=210&height=260',
        href:'home',
      },{
        src:'//img12.360buyimg.com/jrpmobile/jfs/t13927/226/2090083878/14208/2746192a/5a31dde6Nbba7f26c.png?width=210&height=260',
        href:'home',
      },{
        src:'//img12.360buyimg.com/jrpmobile/jfs/t9703/119/296348375/11253/b9bc3ce7/59cb637dNf25b0dff.jpg?width=210&height=260',
        href:'home',
      }],
      options: {
          slidesPerView: 2.8,
          spaceBetween: 24,
      }
    }
  }
}
</script>

<style lang="scss">
.inslider{
  padding-bottom: 40px;
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
          height: 308;
          border: 1px solid red;
        }
      }
    }
  }

}
</style>

<style lang="scss" module>
.car {


  img {
    width:100%;
  }
}
</style>
