<template>
  <div id="app">
    <Navbar/>
    <ImgSlider />
    <Views />
    <Movies />
    <Footer />
  </div>
</template>

<script>
import Navbar from '@/components/Navbar'
import ImgSlider from '@/components/ImgSlider'
import Views from '@/components/Views'
import Movies from '@/components/Movies'
import Footer from '@/components/Footer'



export default {
  name: 'App',
  components: {
    Navbar,
    ImgSlider,
    Views,
    Movies,
    Footer
  }
}
</script>

<style>
 html,body{
   width: 100%;
   background-color: #161924;
 }
</style>
