<template>
  <div class="background">
  <NavBar />
      <h1 class="heading">About Me</h1>
      <div class="bg-container d-flex">
        <div class="card" style="width: 60rem; height: 35rem;padding-top: 5px;">
          <div class="card-body">
            <div class="row align-items-center">
              <div class="col-sm-6 col-md-6 col-lg-6">
                <img src="https://i.postimg.cc/q7XzWw3F/DSC-3548-3.jpg" class="d-block w-100 h-100" alt="anime" width="100%"
                  height="100%">
              </div>
              <div class="col-sm-5 col-md-5 col-lg-5 aboutText">
                  <div class="card-body">
                    <h6 class="text-start">
                      I have always been interested in computers because I was surrounded with friends whom built their own PC's. I started gaming when I was younger and introduced myself to anime. I am an artist, surfer and kickboxer. I started digital art at the beginning of 2022 after years of being an artist I started to teach myself to animate on blender and bring those drawings and paintngs to life. Presently I am a Full-Stack Developer at Life Choices. Learning different programming languages on the side including python, cloud computing and machine learning.
                    </h6>
                  </div>
              </div>
            </div>
            
          </div>
        </div>
      </div>
      <Footer1 />
      
  </div>
 
</template>

<script>
import NavBar from '@/components/Navbar.vue'
import Footer1 from '@/components/Footer.vue'
import CarouselVue from '@/components/Carousel.vue'
export default {
  components: {
    NavBar,
    CarouselVue,
    Footer1
  }
}
</script>

<style scoped>
@import url("https://fonts.googleapis.com/css2?family=Cinzel+Decorative:wght@900&display=swap");


.heading {
  font-family: "Share Tech Mono", monospace;

}

.row {
  padding-top: 10%;
  justify-content: space-around;
}

.aboutText{
  box-shadow: 0 4px 8px 0 rgba(0, 0, 0, 0.2),
    0 6px 20px 0 rgba(0, 0, 0, 0.19);}

@media screen (max-width: 600px) {

  .card {
    border: none;
  }
  
}

</style>
