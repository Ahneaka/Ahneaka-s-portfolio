<template>
  <div class="background">
    <div class="bg-container d-flex justify-content-center">
      <div class="card my-auto" style="width: 60rem; height: 35rem">
        <div class="card-body">
          <NavBar />
          <Home />
        </div>
      </div>
    </div>
    <footer1 />
  </div>
</template>



<script>
// @ is an alias to /src
// import HelloWorld from '@/components/HelloWorld.vue'
// import NavBar from '@/components/Navbar.vue'
import footer1 from '@/components/Footer.vue';
import Home from '@/components/Home.vue';
import NavBar from "@/components/Navbar.vue";

export default {
  name: 'HomeView',
  components: {
    Home,
    footer1,
    NavBar
  }
}
</script>
<style >
    @import url("https://fonts.googleapis.com/css2?family=Cinzel+Decorative:wght@900&display=swap");
body {
  background-size: cover;
  /* background-color: #fff; */
  /* width: 100%; */
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

/* .words {
  padding-top: 10%;
} */


nav a {
  color: rgb(69, 68, 68);
  text-decoration: none;
  font-size: 17px;
}

.nav-img {
  width: 20%;
  height: auto;
  margin-left: 0;
  border-radius: 50%;
  float: left;
}

@media screen and (max-width: 767px) {
  .nav-img {
    width: 15%;
    height: auto;
    margin-left: 0;
    border-radius: 50%;
  }
}

nav a:hover {
  background-color: rgba(128, 128, 128, 0.172);
  color: white;
  border-radius: 25px;
  border: solid 1px;
  border-color: rgb(128, 128, 128);
}



.card-content {
  justify-content: space-around;
}

.words {
      padding-top: 20%;
    }

    h6 {
      letter-spacing: 6px;
      color: #fff;
      font-family: "Cinzel Decorative", cursive;
    }

    h5 {
      font-family: "Share Tech Mono", monospace;
    }

</style>
