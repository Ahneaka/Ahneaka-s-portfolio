<template>
  <!-- <div class="background">
    <NavBar />
    <h1 class="heading">Projects</h1>
    <div class="bg-container d-flex">
      <div class="card my-auto" style="width: 60rem; height: 35rem">
        <div class="card-body">
          
           
        <Footer1 />
      </div>
      </div>
      </div>
      </div> -->
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