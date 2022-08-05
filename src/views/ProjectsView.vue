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
      <h3>A note about style</h3>
      <p>Lorem ipsum dolor sit, amet consectetur adipisicing elit. Quisquam, reprehenderit.</p>
      <a href="">Read more</a>
    </div>
    <div class="tall">
      <img src="" alt="model">
    </div>
    <div class="short">
      <h3>A note about style</h3>
      <p>Lorem ipsum dolor sit, amet consectetur adipisicing elit. Quisquam, reprehenderit.</p>
      <a href="">Read more</a>
    </div>
    <div class="tall">
      <img src="img/2.png" alt="model">
    </div>
    <div class="tall">
      <img src="img/3.png" alt="model">
    </div>
    <div class="tall">
      <h3>A note about style</h3>
      <p>Lorem ipsum dolor sit, amet consectetur adipisicing elit. Quisquam, reprehenderit.</p>
      <p>Lorem ipsum dolor, sit amet consectetur adipisicing elit. Quas perspiciatis natus sit dicta repellendus quia mollitia. Voluptas ullam ipsa dolorem.</p>
      <p>Lorem ipsum dolor, sit amet consectetur adipisicing elit. Esse accusamus possimus asperiores fugiat at nostrum odio repellendus voluptates. Iusto asperiores voluptate similique maiores ut omnis dolores corporis, tenetur excepturi quis?</p>
      <a href="">Read more</a>
    </div>
    <div class="short">
      <h3>A note about style</h3>
      <p>Lorem ipsum dolor sit, amet consectetur adipisicing elit. Quisquam, reprehenderit.</p>
      <a href="">Read more</a>
    </div>
    <div class="tall">
      <img src="img/1.png" alt="model">
    </div>
    <div class="short">
      <h3>A note about style</h3>
      <p>Lorem ipsum dolor sit, amet consectetur adipisicing elit. Quisquam, reprehenderit.</p>
      <a href="">Read more</a>
    </div>
    <div class="short">
      <h3>A note about style</h3>
      <p>Lorem ipsum dolor sit, amet consectetur adipisicing elit. Quisquam, reprehenderit.</p>
      <a href="">Read more</a>
    </div>
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

  main img {
    min-width: 100%;
    height: 100%;
  }

  main .short {
    grid-row: span 1;
  }

  main .tall {
    grid-row: span 2;
 }

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