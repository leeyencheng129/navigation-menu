<template>
  <swiper
    :slides-per-view="1"
    :space-between="0"
    navigation
    :pagination="{ clickable: true }"
     :centeredSlides="true"
     :loop="true"
     :autoplay="{
      delay: 2500,
      disableOnInteraction: false,
    }"
   :breakpoints="{
      '640': {
        slidesPerView: 2,
        
      },
    }"
    :modules="modules"
    @swiper="onSwiper"
    @slideChange="onSlideChange"
  >
    <swiper-slide>
    <img src="../assets/slider/img_01.jpg" class="pc">
    <img src="../assets/slider/img_01_sp.jpg" class="sp">
    </swiper-slide>
    <swiper-slide>
      <img src="../assets/slider/img_02.jpg" class="pc">
        <img src="../assets/slider/img_02_sp.jpg" class="sp">
    </swiper-slide>
    <swiper-slide>
      <img src="../assets/slider/img_03.jpg" class="pc">
        <img src="../assets/slider/img_03_sp.jpg" class="sp">
    </swiper-slide>
   
   
  </swiper>
</template>
<script>
// import Swiper core and required components
import SwiperCore, { Autoplay , Navigation, Pagination, A11y } from "swiper";

// Import Swiper Vue.js components
import { Swiper, SwiperSlide } from "swiper/vue";

// Import Swiper styles
import "swiper/swiper.scss";
import "swiper/components/navigation/navigation.scss";
import "swiper/components/pagination/pagination.scss";

// install Swiper components
SwiperCore.use([Autoplay, Navigation, Pagination, A11y]);

// Import Swiper styles
export default {
  components: {
    Swiper,
    SwiperSlide,
  },
  methods: {
    onSwiper() {
      // console.log(swiper)
    },
    onSlideChange() {
      // console.log('slide change')
    },
  },
};
</script>
<style scoped lang="scss">
.swiper-container{
  width: 100%;
}
img{
  width: 100%;
 
}
:deep(.swiper-pagination-bullet){
  border-radius: 0 ;
}
.swiper-container{
  overflow: inherit;
  @media (max-width:600px){
     overflow: hidden;
  }
}
:deep(.swiper-pagination){
  bottom: -15%;
}
 
  

</style>