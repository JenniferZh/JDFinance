<template lang="html">
    <div>
        <Heador/>
        <Slider/>
        <Novice/>
        <Borrow></Borrow>
    </div>
</template>

<script>
import Heador from '../public/header.vue'
import Slider from '../home/hslider.vue'
import Novice from '../home/novice.vue'
import Borrow from '../home/borrow.vue'
export default {
  components: {
    Heador,
    Slider,
    Novice,
    Borrow,
  }
}
</script>

<style lang="scss" module>

</style>
