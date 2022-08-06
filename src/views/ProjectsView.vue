<template>
<div class="projects">
  <!-- Banner -->
     <div class="banner">
      <div class="banner-text-container">
        <h1>Приключени проекти</h1>
      </div>
    </div>

  <!-- Projects -->
  <main>
    <div class="short">
      <h3>Cryptocoin</h3>
      <p>Уеб сайт за проследяване на цените на криптоактиви. Неговата мисия е да предостави на потребителите висококачествена и точна информация за изготвяне на собствени информирани заключения.</p>
      <a href="http://wine-project.net/" target="_blank">
          <button class="info-btn" >Виж повече</button>
      </a>
    </div>
    <div class="tall">
      <img src="" alt="site-img">
    </div>
    <div class="short">
      <h3>Wine Project</h3>
      <p>ВАЙН ПРОДЖЕКТ ЕООД извършва проектиране, внедряване и поддръжка на съвременни ИТ решения, базирани на широка гама от продукти и решения на утвърдени световни производители.</p>
      <a href="http://wine-project.net/" target="_blank">
          <button class="info-btn" >Виж повече</button>
      </a>
    </div>
    <div class="tall">
      <img src="" alt="site-img">
    </div>
    <div class="tall">
      <img src="" alt="site-img">
    </div>
    <div class="tall">
      <h3>Wine Project</h3>
      <p>ВАЙН ПРОДЖЕКТ ЕООД извършва проектиране, внедряване и поддръжка на съвременни ИТ решения, базирани на широка гама от продукти и решения на утвърдени световни производители.</p>
      <a href="http://wine-project.net/" target="_blank">
          <button class="info-btn" >Виж повече</button>
      </a>
    </div>
    <div class="short">
      <h3>A note about style</h3>
      <p>Lorem ipsum dolor sit, amet consectetur adipisicing elit. Quisquam, reprehenderit.</p>
      <a href="">Read more</a>
    </div>
    <!-- <div class="tall">
      <img src="img/1.png" alt="model">
    </div> -->
    <div class="short">
      <h3>A note about style</h3>
      <p>Lorem ipsum dolor sit, amet consectetur adipisicing elit. Quisquam, reprehenderit.</p>
      <a href="">Read more</a>
    </div>
    <!-- <div class="short">
      <h3>A note about style</h3>
      <p>Lorem ipsum dolor sit, amet consectetur adipisicing elit. Quisquam, reprehenderit.</p>
      <a href="">Read more</a>
    </div> -->
  </main>
</div>
</template>

<script>
export default {
 name:'ProjectsView',
}
</script>

<style scoped>
  /* Banner */
  .banner {
  height: 425px;
  background: url('../assets/banner.jpg');
  background-size: 1050px;
  object-fit: contain;
  display: flex;
  flex-direction: row;
  justify-content: center;
  align-items: center;
}

.banner-text-container {
  width: 100%;
  height: 100%;
  background: rgb(0, 0, 0, 0.5);
  color: #fff;
  line-height: 0.1rem;
  display: flex;
  flex-direction: column;
  justify-content: center;
  align-items: center;
}


  /* Projects */
  main {
    max-width: 1200px;
    margin: 60px auto;
    padding: 20px;
    display: grid;
    grid-template-columns: 1fr 1fr 1fr;
    grid-auto-rows: 250px;
    gap: 30px;
  }

  main div {
    overflow: hidden;
    padding: 1rem;
    background: #fff;
    border: 1px solid #000;
    box-shadow: 3px 3px 5px rgba(0,0,0,0.05);
  }

  div h3 {
    margin: 0.5rem 0;
  }

  main img {
    min-width: 100%;
    /* height: 100%; */
  }

  main .short {
    grid-row: span 1;
  }

  main .tall {
    grid-row: span 2;
 }

  .info-btn {
    cursor: pointer;
    padding: 0.5rem 0.5rem;
    color: #fff;
    background: #000;
    border: 1px solid #fff;
    transition:  0.2s;
  }

  .info-btn:hover {
    padding: 0.5rem 0.5rem;
    color: #000;
    background: #fff;
    border: 1px solid #000;
    transition:  0.2s;
  }

  /* Responsive */

  @media screen and (max-width: 960px) {
    main {
      grid-template-columns: 1fr 1fr;
    }
  }

  @media screen and (max-width: 620px) {
    main {
      grid-template-columns: 1fr;
      max-width: 400px;
      margin-top: 20px;
    }
    nav {
      grid-template-columns: repeat(4, 1fr);
    }
    nav h1{
      grid-column: 1 / span 4;
      grid-row: 1;
    }  
  }

  @media only screen and (max-width: 600px) {

    .banner-text-container h1 {
      font-size: 1.5rem;
    }

  }
</style>