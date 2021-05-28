<template>
    <div class="responsive">
        <VueSlickCarousel v-bind="settings">
            <div>
                <img src="../assets/banner1.jpg" />
            </div>
            <div>
                <img src="../assets/banner2.jpg" />
            </div>
            <div>
                <img src="../assets/banner3.jpg" />
            </div>
        </VueSlickCarousel>
    </div>
</template>

<script>
import VueSlickCarousel from 'vue-slick-carousel'
import 'vue-slick-carousel/dist/vue-slick-carousel.css'
import 'vue-slick-carousel/dist/vue-slick-carousel-theme.css'
    export default {
    data() {
      return {
        settings: {
        "dots": true,
        "dotsClass": "slick-dots custom-dot-class",
        "edgeFriction": 0.35,
        "infinite": true,
        "speed": 500,
        "autoplaySpeed": 2000,
        "slidesToShow": 1,
        "slidesToScroll": 1
        },
      }
    },
    components:{VueSlickCarousel}
  }
</script>

<style lang="css" scoped>
.responsive{
    width: 96%;
    height: 50%;
}

div{
    height: 400px;
    width: 95%;
    margin-top: 20px;
    margin-left: 40px;
}
img{
    width: 100%;;
    height: 90%;
    border-radius: 4px;
    box-shadow: rgb(0 0 0 / 69%) 0px 26px 30px -10px;
   
}
.slick-dots li button::before{
    font-size: 12px;
    color:#fff;
    
}

@media screen and (max-width: 990px){
    .responsive{
        width:90%
    }
}
@media screen and (max-width: 620px){
    .responsive{
        width:80%;
        height: 50%
    }
}
</style>