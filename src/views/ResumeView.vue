<template>
  <div class="background">
    <NavBar />
    <h1 class="heading">Resume</h1>
    <!-- <div class="bg-container d-flex">
      <div class="card my-auto" style="width: 60rem; height: 35rem">
        <div class="card-body"> -->

    <div class="container">
      <div class="row " >
        <div class="col-12 my-3" v-for="item in Education" :key="item">
          <div class="card">
            <img :src="item.image" class="card-img-top" alt="uvyt" width="100" height="500">
            <br>
            <div class="card-body">
              <h3 class="card-title"><span style="color: grey">{{ item.year }}</span><br>{{ item.name }}</h3>

              <h3 class="card-text">{{ item.text }}</h3>
              <br>
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
export default {
  name: 'info',
  data() {
    return {
      Education: [
        {
          year: '2022-2023',
          name: 'Windsor Highschool',
          text: 'National Certificate',
          image: 'https://i.postimg.cc/yNTh5J4g/windsor.jpg'
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

.container{
  width: 60%;
}
.Section2{
  padding-top: 50%;
}

img{
  width: 100%;
  max-width: 300px;
  height: 250px;
  min-height: 200px;
  align-self: center;
}
.card{
  display: flex;
  padding-top: 1em;
}
@media screen and (max-width:768px) {

  img{
    width: 50%;
    min-width: 250px;
    max-width: 40%;
    height: auto;
    align-self: center;
  }
}


</style>