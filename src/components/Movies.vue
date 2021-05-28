<template>
    <Container>
        <h3>Recommended for You</h3>
        <VueSlickCarousel v-bind="settings">
            <div><img src="../assets/banner2.jpg"></div>
            <div><img src="../assets/banner1.jpg"></div>
            <div><img src="../assets/banner3.jpg"></div>
            <div><img src="../assets/banner3.jpg"></div>
            <div><img src="../assets/banner2.jpg"></div>
            <div><img src="../assets/banner1.jpg"></div>
        </VueSlickCarousel>
        <h3>News on Disney +</h3>
        <VueSlickCarousel v-bind="settings">
            <div><img src="../assets/banner2.jpg"></div>
            <div><img src="../assets/banner1.jpg"></div>
            <div><img src="../assets/banner3.jpg"></div>
            <div><img src="../assets/banner3.jpg"></div>
            <div><img src="../assets/banner2.jpg"></div>
            <div><img src="../assets/banner1.jpg"></div>
        </VueSlickCarousel>
    </Container>
</template>

<script>
import VueSlickCarousel from 'vue-slick-carousel'
import 'vue-slick-carousel/dist/vue-slick-carousel.css'
import 'vue-slick-carousel/dist/vue-slick-carousel-theme.css'
    export default {
        data() {
            return {
                settings:{
                    "infinite": true,
                    "slidesToShow": 5,
                    "speed": 500,
                    "rows": 1,
                    "slidesPerRow": 1
                }
            }
        },
        components:{VueSlickCarousel}
        
    }
</script>

<style lang="css" scoped>
Container{
    margin: 30px;
    color:#fff;
}
Container h3{
    padding: 20px 0 0 80px
}
div{
    height: 250px;
    width: 95%;
    margin-top: 10px;
    margin-left: 30px;  
}

div img{
    margin-top: 20px;
    padding: 5px;
    width: 100%;
    height: 150px;
    border-radius:4px;
    box-shadow: rgb(0 0 0/ 69%) 0px 26px 30px -10px,rgb(0 0 0 /73%) 0px 16px 10px -10px; 
}

</style>