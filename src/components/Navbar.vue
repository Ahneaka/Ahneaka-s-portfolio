<template>
  <nav class="navbar navbar-expand-md">
    <div class="container">
      <div class="d-flex">
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
  </nav>
</template>

<script>
export default {
  name: 'NavBar'
}
</script>

<style>
.navbar>.container,
.navbar>.container-fluid,
.navbar>.container-lg,
.navbar>.container-md,
.navbar>.container-sm,
.navbar>.container-xl,
.navbar>.container-xxl {
  justify-content: end !important;
}</style>