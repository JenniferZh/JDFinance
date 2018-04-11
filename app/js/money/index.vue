<template lang="html">
    <div>
        <Heador/>
        <Slider/>
        <Ada></Ada>
        <Money></Money>
        <Adb></Adb>
        <Select></Select>
        <Footer></Footer>
        <Navbar></Navbar>
    </div>
</template>

<script>
import Heador from '../public/header.vue'
import Slider from './mslider.vue'
import Ada from './ada.vue'
import Adb from './adb.vue'
import Money from './money.vue'
import Select from './select.vue'
import Footer from '../public/footer.vue'
import Navbar from '../public/navbar.vue'
export default {
  components: {
    Heador,
    Slider,
    Money,
    Footer,
    Navbar,
    Ada,
    Adb,
    Select,
  }
}
</script>

<style lang="scss" module>

</style>
