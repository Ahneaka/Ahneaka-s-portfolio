<template>
    <information/>
    <Footer1/>
</template>

<script>
import NavBar from '@/components/Navbar.vue'
import Footer1 from '@/components/Footer.vue'
import information from '@/components/projects.vue'
export default {
  name: 'Project',
  components: {
    NavBar,
    Footer1,
    information
  }
}

</script>

