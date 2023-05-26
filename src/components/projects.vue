<template>
    <div class="background">
        <NavBar />
        <h1 class="heading">Projects</h1>
        <!-- <div class="bg-container d-flex">
            <div class="card my-auto" style="width: 60rem; height: 35rem">
                <div class="card-body">
                    <div id="carouselExampleCaptions" class="carousel slide my-5" data-bs-ride="carousel">
                        <div class="carousel-indicators">
                            <button type="button" data-bs-target="#carouselExampleCaptions" data-bs-slide-to="0"
                                class="active" aria-current="true" aria-label="Slide 1"></button>
                            <button type="button" data-bs-target="#carouselExampleCaptions" data-bs-slide-to="1"
                                aria-label="Slide 2"></button>
                            <button type="button" data-bs-target="#carouselExampleCaptions" data-bs-slide-to="2"
                                aria-label="Slide 3"></button>
                            <button type="button" data-bs-target="#carouselExampleCaptions" data-bs-slide-to="3"
                                aria-label="Slide 4"></button>
                            <button type="button" data-bs-target="#carouselExampleCaptions" data-bs-slide-to="4"
                                aria-label="Slide 5"></button>
                            <button type="button" data-bs-target="#carouselExampleCaptions" data-bs-slide-to="5"
                                aria-label="Slide 6"></button>
                        </div>
                        <div class="carousel-inner">
                            <div class="carousel-item active" v-for="item in Projects2" :key="item">
                                <a :href="item.site"><img :src="item.image" class="d-block w-100" :alt="item.name"> </a>
                                <div class="carousel-caption d-none d-md-block">
                                    <h1>{{ item.name }}</h1>

                                </div>
                            </div>
                            <div class="carousel-item" v-for="item in Projects" :key="item" >
                                <a :href="item.site"><img :src="item.image" class="d-block w-100" :alt="item.name"> </a>
                                <div class="carousel-caption d-none d-md-block">
                                    <h1>{{ item.name }}</h1>

                                </div>
                            </div>

                            <div class="carousel-item">
                                <a href="https://v-v-g-exhibit.netlify.app/"><img src="" class="d-block w-100" alt=""
                                        width="100%" height="100%"> </a>
                                <div class="carousel-caption d-none d-md-block">
                                </div>
                            </div>
                            <div class="carousel-item">
                                <a href="https://aniimeflix-anime.netlify.app/"><img src="" class="d-block w-100" alt=""
                                        width="100%" height="100%"> </a>
                                <div class="carousel-caption d-none d-md-block">
                                </div>
                            </div>

                            <button class="carousel-control-prev" type="button"
                                data-bs-target="#carouselExampleCaptions" data-bs-slide="prev">
                                <span class="carousel-control-prev-icon" aria-hidden="true"></span>
                                <span class="visually-hidden">Previous</span>
                            </button>
                            <button class="carousel-control-next" type="button"
                                data-bs-target="#carouselExampleCaptions" data-bs-slide="next">
                                <span class="carousel-control-next-icon" aria-hidden="true"></span>
                                <span class="visually-hidden">Next</span>
                            </button>
                        </div>
                    </div>
                </div>
            </div>

        </div> -->
<div class="container">
    <div class="row">
  <div class="col-md-4 my-3 align-self-start" v-for="item in Projects" :key="item">
    <div class="card">
        <div class="card-body">
            <img class="card-img-top" :src="item.image" style="height: 200px; width: 300px;"  alt="">
            <h3 class="card-text">{{item.name }} </h3>
          <a :href="item.site" target="_blank" class="btn btn-secondary">View Project
        </a>
        </div>
      </div>
  </div>
    </div> 
</div>
    </div>
</template>

<script>
import NavBar from '@/components/Navbar.vue'
import Footer1 from '@/components/Footer.vue'
export default {
    name: 'information',
    data() {
        return {
            Projects: [
                {
                    name: 'Arcadian',
                    class: 'active',
                    image: 'https://i.postimg.cc/7PKBJnkf/Screenshot-2023-05-10-091927.png',
                    site: 'https://arcadian-ea31c.web.app/'
                },
                {
                    name: 'Cypher',
                    image: 'https://i.postimg.cc/wjFVztKg/Screenshot-2023-04-18-151741.png',
                    site: 'https://cypher-4e67a.web.app/'
                },
    
                {
                    name: 'Supwave',
                    image: 'https://i.postimg.cc/QdsFbSyd/Screenshot-2023-04-18-151912.png',
                    site: 'https://supwave-shop.netlify.app/'
                },
                {
                    name: 'Old portfolio',
                    image: 'https://i.postimg.cc/g27bqR1F/Screenshot-4.png',
                    site: 'https://old-profile.netlify.app/'
                },
                {
                    name: 'Calculater',
                    image: 'https://i.postimg.cc/RVCh8GBs/Screenshot-2023-04-18-151847.png',
                    site: 'https://new-calculator-ahneaka.netlify.app/'
                },
                {
                    name: 'Aniimeflix',
                    image: 'https://i.postimg.cc/QVLjb7Fd/Screenshot-3.png',
                    site: 'https://aniimeflix-anime.netlify.app/'
                }

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

.row{
    align-items: center;
    justify-content: center;
}
.carousel-item {
    /* height: 30rem; */
    color: pink;
    /* background-color: gold; */
    display: flex;
    justify-content: center;
    align-content: center;
}

@media (max-width: 1200px) { 
     .card-img-top{
        width: 250px !important; 
    }
    
}

@media (max-width: 997px) { 
     .card-img-top{
        width: 170px !important; 
    }
    
}

@media (max-width: 900px) { 
     .card-img-top{
        width: 180px !important; 
    }
    
}

</style>