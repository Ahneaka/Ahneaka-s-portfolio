<template>
  <div class="background">
    <NavBar />
    <h1 class="heading">About Me</h1>
    <div class="bg-container d-flex">
      <div class="card my-auto" style="width: 60rem; height: 35rem">
        <div class="card-body">
          <div class="row">
            <div class="col-md-6">
              <img src="https://i.postimg.cc/q7XzWw3F/DSC-3548-3.jpg" class="d-block w-100 h-100" alt="anime" width="100%"
                height="100%">
            </div>
            <div class="col-md-6">
              <div class="card my-auto" style="width: 25rem; height: 20rem">
                <div class="card-body">
                  <h6>
                    I have always been interested in computers because I was surrounded with friends whom built their own PC's. I started gaming when I was younger and introduced myself to anime. I am an artist, surfer and kickboxer. I started digital art at the beginning of 2022 after years of being an artist I started to teach myself to animate on blender and bring those drawings and paintngs to life. Presently I am a Full-Stack Developer at Life Choices. Learning different programming languages on the side including python, cloud computing and machine learning.
                  </h6>
                </div>
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

/* .background {
  background-image: url(../assets/backgroundimg.jpg);
  background-size: cover ;
  width: 100%;
  height: 100%;
} */
.heading {
  font-family: "Share Tech Mono", monospace;

}

.row {
  padding-top: 10%;
}
@media screen and (max-width:650px) {

img {
  /* width: 250px; */
  min-width: 150px;
  max-width: 165px;
  height: auto;
  align-self: center;
}

.card {
  min-width: 200px;
  max-width: 165px;
  height: auto;
  align-self: center;
  justify-content: center;
}


}


/* @media screen and (max-width:900px) {
.h6{

}
  .card{
    width: 50px;
  min-width: 270px;
  max-width: 40px;
  height: 50px;
  align-self: center;
  }

} */

</style>
