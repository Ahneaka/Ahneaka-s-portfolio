<template>
  <div class="background">
    <NavBar />
    <body>
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
      
    </body>
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
}
@media screen and (max-width:650px) {

img {
  min-width: 150px;
  max-width: 165px;
  height: 178px;
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


body {
  background-size: cover;
  background-image: linear-gradient(45deg,
      rgba(181, 63, 83, 0.952),
      pink,
      rgb(177, 177, 177),
      rgba(255, 154, 143, 0.68),
      pink,
      rgb(149, 149, 149));
  background-size: 200%, 100%;
  animation: bgAnimationGradient 4s infinite linear;
}

@keyframes bgAnimationGradient {
  0% {
    background-position: 0 0;
  }

  100% {
    background-position: 100% 0;
  }
}

.flex-container {
  position: relative;
  right: 0;
  top: 80px;
  float: left;
  display: flex;
  flex-direction: row;
  justify-content: left;
}

.bg-container {
  padding-top: 5rem;
}

.card {
  margin: auto;
  justify-content: center;
  box-shadow: 0 4px 8px 0 rgba(0, 0, 0, 0.2),
    0 6px 20px 0 rgba(0, 0, 0, 0.19);
  background-color: transparent !important;
  backdrop-filter: blur(10px);
}

/* Media queries for 300px and 700px */
@media screen and (max-width: 700px) {
  .card {
    width: 90%;
    height: auto;
  }

  .card.my-auto {
    width: 100%;
    height: auto;
  }

  .row {
    flex-direction: column;
  }
}

@media screen and (max-width: 300px) {
  .card {
    width: 100%;
    height: auto;
  }

  .card.my-auto {
    width: 100%;
    height: auto;
  }

  .row {
    flex-direction: column;
  }
}

</style>
