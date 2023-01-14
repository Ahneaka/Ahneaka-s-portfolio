<template>
    <div class="background">
      <NavBar/>
      <h1>Testimonials</h1>
      <TestimonialsVue></TestimonialsVue>

            <Footer1/>

    </div>
</template>

<script>
import NavBar from '@/components/Navbar.vue';
import TestimonialsVue from '@/components/Testimonials.vue';
import Footer1 from '@/components/Footer.vue'
export default{
  components: {
    NavBar,
    TestimonialsVue,
    Footer1
  }
}

</script>
