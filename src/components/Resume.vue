<template>
    <div class="background">
    <div class="bg-container d-flex justify-content-center">
      <div class="card my-auto" style="width: 60rem; height: 35rem">
        <div class="card-body">
          <NavBar />
          <div class="name">
            <div class="year">
              <div class="image">
                
              </div>
            </div>
          </div>
        </div>
      </div>
    </div>
    </div>
</template>

<script>

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
  }
  }
</script>
