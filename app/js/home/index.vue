<template lang="html">
    <div>
        <Heador/>
        <Slider/>
        <Novice/>
        <Borrow></Borrow>
        <Money></Money>
        <Product></Product>
        <Insurance></Insurance>
        <Footer></Footer>
        <Navbar></Navbar>
    </div>
</template>

<script>
import Heador from '../public/header.vue'
import Slider from '../home/hslider.vue'
import Novice from '../home/novice.vue'
import Borrow from '../home/borrow.vue'
import Money from '../home/money.vue'
import Product from '../home/product.vue'
import Insurance from '../home/insurance.vue'
import Footer from '../public/footer.vue'
import Navbar from '../public/navbar.vue'
export default {
  components: {
    Heador,
    Slider,
    Novice,
    Borrow,
    Money,
    Product,
    Insurance,
    Footer,
    Navbar,
  }
}
</script>

<style lang="scss" module>

</style>
