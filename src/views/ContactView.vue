<template>
  <div class="background">
    <NavBar />
    <h1 class="heading">Contact</h1>
    <div class="bg-container d-flex">
      <div class="card my-auto" >
        <div class="card-body">
          <form action="https://formspree.io/f/myyvjoyz" method="post" class="row g-3 needs-validation" novalidate>
            <div class="col-md-6 position-relative">
              <label for="validationTooltip01" class="form-label">First name</label>
              <input type="text" name="name" class="form-control" id="validationTooltip01" value="" required>
              <div class="valid-tooltip">
                Looks good!
              </div>
            </div>
            <div class="col-md-6 position-relative">
              <label for="validationTooltip02" class="form-label">Last name</label>
              <input type="text" name="surname" class="form-control" id="validationTooltip02" value="" required>
              <div class="valid-tooltip">
                Looks good!
              </div>
            </div>
            <div class="col-md-12 position-relative">
              <label for="validationTooltipUsername" class="form-label">Email</label>
              <div class="input-group has-validation">
                <span class="input-group-text" id="validationTooltipUsernamePrepend">@</span>
                <input type="text" name="username" class="form-control" id="validationTooltipUsername"
                  aria-describedby="validationTooltipUsernamePrepend" required>
                <div class="invalid-tooltip">
                  Please choose a unique and valid username.
                </div>
              </div>
            </div>
            <div class="col-md-12 position-relative">
              <label for="validationTooltip03" class="form-label">Comment</label>
              <textarea type="text" name="message" class="form-control" id="validationTooltip03" value="" required style="height: 5rem;"></textarea>
            </div>
            <div class="col-12 pt-3">
              <button class="btn btn-secondary" type="submit">Submit form</button>
            </div>
          </form>
        </div>
      </div>
    </div>
    <Footer1 />
  </div>
</template>

<script>
import NavBar from '@/components/Navbar.vue'
import Footer1 from '@/components/Footer.vue'
export default {
  components: {
    NavBar,
    Footer1
  }
}
</script>

<style>
/* @media screen and (max-width: 601px) {
  .bg-container{
    height: 50rem;
  }
} */

</style>
