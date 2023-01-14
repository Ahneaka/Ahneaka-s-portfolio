<template>
  <!-- <nav class="nav"> -->
  <!-- <img class="nav-img" img src="/img/1667550652766.jpg" width="60px" height="60px" />

        <a class="page-scroll"><router-link to="/">Home</router-link></a>
    
        <a class="page-scroll"><router-link to="/about">About</router-link></a>
    
        <a class="page-scroll"><router-link to="/resume">Resume</router-link></a>
    
        <a class="page-scroll"><router-link to="/project">Projects</router-link></a>
    
        <a class="page-scroll"><router-link to="/testimonials">Testimonials</router-link></a>
    
        <a class="page-scroll"><router-link to="/contact">Contact</router-link></a> -->
  <nav class="navbar navbar-expand-md">
    <div class="container">
      <div class="d-flex">
        <a href="" class="navbar-brand m-auto">
          <img class="nav-img d-inline-block" img src="https://i.postimg.cc/7h5gy5k0/1667550652766.jpg" width="30px"
            height="10px" />
        </a>
        <button class="navbar-toggler" type="button" data-bs-toggle="collapse" data-bs-target="#navbarToggler"
          aria-controls="navbarToggler" aria-expanded="false" aria-label="Toggle navigation">
          <span class="navbar-toggler-icon"></span>
        </button>
      </div>
      <div class="collapse navbar-collapse" id="navbarToggler">
        <ul class="navbar-nav text-center mx-auto mb-2 mb-lg-0">
          <li class="nav-item">
            <a class="page-scroll nav-link"><router-link to="/">Home</router-link></a>
          </li>
          <li class="nav-item">
            <a class="page-scroll nav-link"><router-link to="/about">About</router-link></a>
          </li>
          <li class="nav-item">
            <a class="page-scroll nav-link"><router-link to="/resume">Resume</router-link></a>
          </li>
          <li class="nav-item">
            <a class="page-scroll nav-link"><router-link to="/project">Projects</router-link></a>
          </li>
          <li class="nav-item">
            <a class="page-scroll nav-link"><router-link to="/testimonials">Testimonials</router-link></a>
          </li>
          <li class="nav-item">
            <a class="page-scroll nav-link"><router-link to="/contact">Contact</router-link></a>
          </li>
        </ul>
      </div>
    </div>
    <!-- </nav> -->
  </nav>
</template>

<script>
export default {
  name: 'NavBar'
  }
</script>

<style>

</style>