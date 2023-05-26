<template>
    <div class="background">
        <NavBar />
        <h1 class="heading">Projects</h1>
        <div class="container">
            <div class="row">
                <div class="col-md-4 my-3 align-self-start" v-for="item in Projects" :key="item">
                    <div class="card">
                        <div class="card-body">
                            <img class="card-img-top" :src="item.image" style="height: 200px; width: 300px;" alt="">
                            <h3 class="card-text">{{ item.name }} </h3>
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
.row {
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
    .card-img-top {
        width: 250px !important;
    }

}

@media (max-width: 997px) {
    .card-img-top {
        width: 170px !important;
    }

}

@media (max-width: 900px) {
    .card-img-top {
        width: 180px !important;
    }

}
</style>