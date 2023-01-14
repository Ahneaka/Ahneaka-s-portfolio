<template>
  <div class="background">
    <NavBar />
    <h1 class="heading">Resume</h1>
    <!-- <div class="bg-container d-flex">
      <div class="card my-auto" style="width: 60rem; height: 35rem">
        <div class="card-body"> -->

    <div class="container">
      <div class="row" v-for="item in Education" :key="item">
        <div class="col order-last">
          <div class="card" style="width: 18rem;">
            <img :src="item.image" class="card-img-top" alt="">
            <br>
            <div class="card-body">
              <h3 class="card-title"><span style="color: grey">{{ item.year }}</span><br>{{ item.name }}</h3>

              <h1 class="card-text">{{ item.text }}</h1>
              <br>
            </div>
          </div>
        </div>
        <!-- <div class="col">
      <div class="card" style="width: 18rem;">
                <img src="" class="card-img-top" alt="">
                <div class="card-body">
                  <h3 class="card-title">2022- <span style="color: blue"> False bay college- Muizenburg</span></h3>

                  <h1 class="card-text">Hospitality and Catering practical N6 Certificate</h1>
                </div>
              </div>
    </div>
    <div class="col order-first">
      <div class="card" style="width: 18rem;">
                <img src="" class="card-img-top" alt="">
                <div class="card-body">
                  <h3 class="card-title">2022- <span style="color: green"> Life Choices</span></h3>

                  <h1 class="card-text">Coding</h1>
                </div>
              </div>
    </div> -->
        <!-- </div>
</div> -->
        <!-- <div class="grid">
            <div class="g-col-6 g-col-md-4">
              <div class="card" style="width: 18rem;">
                <img src="" class="card-img-top" alt="">
                <div class="card-body">
                  <h3 class="card-title">2022- <span style="color: green"> Life Choices</span></h3>

                  <h1 class="card-text">Coding</h1>
                </div>
              </div>
            </div>
            <div class="g-col-6 g-col-md-4">
              <div class="card" style="width: 18rem;">
                <img src="" class="card-img-top" alt="">
                <div class="card-body">
                  <h3 class="card-title">2022- <span style="color: blue"> False bay college- Muizenburg</span></h3>

                  <h1 class="card-text">Hospitality and Catering practical N6 Certificate</h1>
                </div>
              </div>
            </div>
            <div class="g-col-6 g-col-md-4">
              <div class="card" style="width: 18rem;">
                <img src="" class="card-img-top" alt="">
                <div class="card-body">
                  <h3 class="card-title">2022- <span style="color: cyan"> Windsor Highschool</span></h3>

                  <h1 class="card-text">National Certificate</h1>
                </div>
              </div>
            </div>
          </div> -->

      </div>
    </div>
  
<section2>
  <h1 class="heading">Skills</h1>
  <div class="bg-container d-flex">
    <div class="card my-auto" style="width: 60rem; height: 35rem">
      <div class="card-body">
        <div class="flex-container">

          <img src="https://i.postimg.cc/bNtBJcVQ/html.png" style="height: 100px; width: 150px;"><br>
          <div class="progress">
            <div class="progress-bar progress-bar-striped progress-bar-animated" role="progressbar" aria-valuenow="75"
              aria-valuemin="0" aria-valuemax="100" style="width: 75%"></div>
          </div>
          <img src="https://i.postimg.cc/vmqJn7r9/css.png" style="height: 100px; width: 150px;"><br>
          <div class="progress">
            <div class="progress-bar progress-bar-striped progress-bar-animated" role="progressbar" aria-valuenow="75"
              aria-valuemin="0" aria-valuemax="100" style="width: 75%"></div>
          </div>
          <img src="https://i.postimg.cc/gcXWv7B0/bootstrap.png" style="height: 150px; width: 160px;">
          <div class="progress">
            <div class="progress-bar progress-bar-striped progress-bar-animated" role="progressbar" aria-valuenow="75"
              aria-valuemin="0" aria-valuemax="100" style="width: 50%"></div>
          </div>
        </div>
      </div>
    </div>

  </div>
</section2>
  <Footer1 />
  </div>
</template>

<script>
import NavBar from '@/components/Navbar.vue'
import Footer1 from '@/components/Footer.vue'
export default {
  name: 'info',
  data() {
    return {
      Education: [
        {
          year: '2022-2023',
          name: 'Windsor Highschool',
          text: 'National Certificate',
          image: 'https://i.postimg.cc/hPmQ3phD/th.jpg'
        },
        {
          year: '2021-2022',
          name: 'False bay college- Muizenburg',
          text: 'Hospitality and Catering practical N6 Certificate',
          image: 'https://i.postimg.cc/25QwRC65/2309876.webp'
        },

        {
          year: '2015-2019',
          name: 'Life Choices',
          text: 'coding',
          image: 'https://i.postimg.cc/SRD10kg9/lc.png'
        },


      ]

    }
  },

  components: {
    NavBar,
    Footer1
  }
}

</script>

<style scoped>
.Section2{
  padding-top: 50%;
}
</style>