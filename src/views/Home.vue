<template>
  <div class="home">
    <Slider></Slider>
    <Slogan></Slogan>
    <Skin></Skin>
    <Beauty></Beauty>
  
  </div>
</template>

<script>
// @ is an alias to /src
import Slider from '../components/Slider.vue'
import Slogan from '../components/Slogan.vue'
import Skin from '../components/Skin.vue'
import Beauty from '../components/Beauty.vue'

export default {
  name: 'Home',
  components: { Slider, Slogan, Skin, Beauty }
}
</script>

<style lang="scss" scoped>
</style>
