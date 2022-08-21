<template>
  <div class="container">
    <h5>Lorem ipsum dolor, sit amet consectetur adipisicing elit. Esse mollitia asperiores expedita quis rem totam minus commodi, nam eligendi beatae?</h5>
    <carousel-3d>
        <slide :index="0" class="slide">
            <h2>Butilkavino</h2>
            <img src="../assets/ButilkavinoText.jpg" alt="">
            <p>Lorem ipsum, dolor sit amet consectetur adipisicing elit. Reiciendis libero harum, reprehenderit pariatur veritatis ducimus!</p>
            <button class="info-btn">Виж още</button>
        </slide>
        <slide :index="1" class="slide">
            <h2>Vremednes</h2>
            <img src="" alt=""></img>
            <p>Lorem ipsum, dolor sit amet consectetur adipisicing elit. Reiciendis libero harum, reprehenderit pariatur veritatis ducimus!</p>
            <button class="info-btn">Виж още</button>
        </slide>
        <slide :index="2" class="slide">
            <h2>Cryptocoin</h2>
            <img src="" alt=""></img>
            <p>Lorem ipsum, dolor sit amet consectetur adipisicing elit. Reiciendis libero harum, reprehenderit pariatur veritatis ducimus!</p>
            <button class="info-btn">Виж още</button>
        </slide>
        <slide :index="3" class="slide">
            <h2>Wine Project</h2>
            <img src="" alt=""></img>
            <p>Lorem ipsum, dolor sit amet consectetur adipisicing elit. Reiciendis libero harum, reprehenderit pariatur veritatis ducimus!</p>
            <button class="info-btn">Виж още</button>
        </slide>
        <slide :index="4" class="slide">
            <h2>Axis</h2>
            <img src="" alt=""></img>
            <p>Lorem ipsum, dolor sit amet consectetur adipisicing elit. Reiciendis libero harum, reprehenderit pariatur veritatis ducimus!</p>
            <button class="info-btn">Виж още</button>
        </slide>
    </carousel-3d>
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
    margin: auto;
    display: flex;
    justify-content: center;
    align-items: center;
    padding: 2rem;
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
</style>