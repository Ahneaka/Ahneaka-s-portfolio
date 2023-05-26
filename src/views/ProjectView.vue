<template>
    <information/>
    <Footer1/>
</template>

<script>
import NavBar from '@/components/Navbar.vue'
import CarouselVue from '@/components/Carousel.vue'
import Footer1 from '@/components/Footer.vue'
import information from '@/components/projects.vue'
export default {
  components: {
    NavBar,
    CarouselVue,
    Footer1,
    information
  }
}

</script>

<style scoped>
.carousel-item {
    height: 32rem;
    color: pink;


  }

</style>