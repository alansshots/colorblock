<template>
  <div class="container">
    <carousel-3d class="carousel" :autoplay="true" :autoplay-timeout="3000" :controls-visible="true" :controls-prev-html="'&#x2039; '" :controls-next-html="'&#x203A;'" :controls-width="10" :controls-height="30" :clickable="false" height="350">
        <slide :index="0" class="slide">
            <h2>Butilkavino</h2>
            <img src="../assets/ButilkavinoText.jpg" alt="butilkavino.com logo">
            <p>Онлайн магазин.</p>
            <p>#Wordpress</p>
            <a href="https://butilkavino.com/" class="info-btn">Виж още</a>
        </slide>
        <slide :index="1" class="slide">
            <h2>Vremednes</h2>
            <img src="../assets/vremedneslogo.png" alt="vremednes logo"></img>
            <p>Уеб приложение</p>
            <p>#HTML #CSS #JavaScript </p>
            <a href="http://vremednes.colorblockweb.com/" class="info-btn">Виж още</a>
        </slide>
        <slide :index="2" class="slide">
            <h2>Cryptocoin</h2>
            <img src="../assets/cryptologo.png" alt="cryptocoin logo"></img>
            <p>Уеб приложение</p>
            <p>#TailwindCSS #Vue.js #Axios</p>
            <a href="http://cryptocoin.colorblockweb.com/" class="info-btn">Виж още</a>
        </slide>
        <slide :index="3" class="slide">
            <h2>Wine Project</h2>
            <img src="../assets/winelogo.png" alt="wine project logo"></img>
            <p>Статичен уебсайт</p>
            <p>#TailwindCSS</p>
            <a href="http://wine-project.net/" class="info-btn">Виж още</a>
        </slide>
        <slide :index="4" class="slide">
            <h2>Axis</h2>
            <img src="../assets/axislogo.png" alt="axis logo"></img>
            <p>Уеб приложение</p>
            <p>#TailwindCSS #JS #PHP #Laravel</p>
            <a href="http://3dprint.webimpression.net/home" class="info-btn">Виж още</a>
        </slide>
    </carousel-3d>
    <div class="container">
      <p>Свържете се с нас, за да разговаряте със специалист или да научите повече за услугите, които предлагаме. Нaшата цел е да Ви помогнем да намерите правилното решение, което да отговаря на Вашите нужди.</p>
      <router-link to="/contact">
      <button class="info-btn">Контакти</button>
      </router-link>
    </div>  
  </div>
</template>

<script>
import { Carousel3d, Slide } from 'vue-carousel-3d';
export default {
   name: 'ProjectsComponent',
   components: {
    Carousel3d,
    Slide
    },
}
</script>

<style scoped>
  .container {
    text-align: center;
    margin: auto;
    width: 60%;
    display: flex;
    flex-direction: column;
    justify-content: center;
    align-items: center;
    padding: 1rem;
  }

  .slide {
      background: #fff;
      border: 1px solid #000;
      padding: 10px;
      text-align: center;
  }

  .slide img {
    width: 200px;
  }

  .info-btn {
    margin-top: 0.5rem;
    cursor: pointer;
    padding: 0.5rem 2rem;
    color: #fff;
    background: #000;
    border: 1px solid #fff;
    transition:  0.2s;
  }

  .info-btn:hover {
    padding: 0.5rem 2rem;
    color: #000;
    background: #fff;
    border: 1px solid #000;
    transition:  0.2s;
  }

  @media only screen and (max-width: 768px) {
   .container {
    width: 100%;
  }

  .slide img {
    width: 120px;
  }
 
}
</style>