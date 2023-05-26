<template>
    <div class="background">
    <div class="container-fluid bg-container d-flex justify-content-center">
      <div class="card my-auto" style="width: 60rem; height: 35rem">
        <div class="card-body">
          <NavBar />
          <!-- <button id="download-btn" @click="downloadCV">Download my CV</button> -->
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
    
    // methods: {
    //   downloadCV() {
    //     const link = document.createElement('a');
    //     link.href = 'https://drive.google.com/file/d/1WMXPg44D5EyBDguxI45QLoRueHbwbwON/view?usp=share_link';
    //     link.download = 'Aneeqa Brown CV and Cover letter.pdf';
    //     link.click()
    //   }
    // },
    
  data() {
    return {
      Education: [
        {
          year: '2015-2019',
          name: 'Windsor Highschool',
          text: 'National Certificate',
          image: 'https://i.postimg.cc/hPmQ3phD/th.jpg'
        },
        {
          year: '2021-2022',
          name: 'False Bay College',
          text: 'Hospitality and Catering practical N6 Certificate',
          image: 'https://i.postimg.cc/25QwRC65/2309876.webp'
        },

        {
          year: '2022-2023',
          name: 'Life Choices',
          text: 'Full-Stack Developer',
          image: 'https://i.postimg.cc/SRD10kg9/lc.png'
        },


      ]

    }
  }
  }
</script>
