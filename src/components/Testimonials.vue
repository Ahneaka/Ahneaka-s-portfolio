<template>
  <div class="container">
    <div class="row">
      <div class="col-md-4 peep my-4 align-self-start"  v-for="testis in Testimonials" :key="testis">
        <div class="card">
            <div class="card-body">
                <img :src="testis.image" style="height: 250px; max-width: 300px;" class="card-img-top" alt="">
                <h3 class="card-text">{{testis.name }} </h3>
              <p class="card-text">{{testis.words }}<br>
                {{testis.email }}
            </p>
            </div>
          </div>
      </div>
        </div>  
          
  </div>
</template>
<script>
export default {
    name: "testis",
    data() {
        return {
            Testimonials: [
                {
                    name: "Nikita Ramawoother",
                    image: "https://i.postimg.cc/595nnWy5/nikita.jpg",
                    words: "Aneeqa is a very creative individual and she is not only helpful but also an exceptional developer that you can always count on to get some ideas and inspiration from.",
                    email: "crazyscientist996@gmail.com"
                },
                {
                    name: "Mu'eed Brown",
                    image: "https://i.postimg.cc/vBtfLMhc/DSC-3535-1.jpg",
                    words: "Aneeqa is a talented individual, she has a creative mind that will allow her to make use of her web development skills. She also has great communication skills, she can work well with  others.",
                    email: "mueedb036@gmail.com"
                },
                {
                    name: "Abdul-Azeez",
                    image: "https://i.postimg.cc/C1GHPbhM/C11-Abdul-Azeez-Kemp-1.jpg",
                    words: "Aneeqa, is a wonderful lady, personality is one of kind, unique. Hard working individual and great to work with and always available with a smile on her face if you need assistance or to just to converse with.",
                    email: "aakemp786@gmail.com"
                },
                {
                    name: "Jake Jansen",
                    image: "https://i.postimg.cc/prybYVvZ/C11-Jake-Jansen-3.jpg",
                    words: "Aneeqa is a super creative and ambitious individual that is very kind and loves to give to others. She has very good taste in development and has a bright future and aneeqa would be a great asset in every company.",
                    email: "jakejanseneagel@gmail.com"
                },
                {
                    name: "Savanah Samuels",
                    image: "https://i.postimg.cc/3RcbhXMX/C11-Savannah-Samuels-1.jpg",
                    words: "Aneeqa is a very diligent and patient person. She works well in teams and is very hardworking. She takes pride in her work and is very efficient. She is very kind hearted and would be a great asset to any company she works at.",
                    email: "savsamuels@gmail.com"
                },
                {
                    name: "Zoe Daniels",
                    image: "https://i.postimg.cc/BQY5VS0F/zozo.jpg",
                    words: "Aneeqa is a hard working lady with a big heart. Her communication skills are excellent no matter if you are talking about verbal or written. Her most important quality is that she always keeps herself updated with new information .",
                    email: "zoedaniels@gmail.com"
                },
            ]
        }
    }
    
}
</script>
<style scoped>

.peep{
    width: 400px;
    height: 450px;

}

.card-body{
    max-height: 500px;
}
    
</style>