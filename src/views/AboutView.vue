<template>
  <div class="about">
    <!-- Banner -->
    <div class="banner">
      <div class="banner-text-container">
        <h1>Научете повече за нас!</h1>
      </div>
    </div>

    <!-- About main -->
    <h2 class="heading">We are a group of creative thinkers reimagining the web.</h2>

    <div class="info-container">
      <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Libero ipsa eveniet doloremque, maiores vero veritatis quisquam ea sit repellat labore consequuntur velit quis eius et iusto? Nisi at numquam suscipit architecto repellat dolor odio accusamus.</p>
      <p>Lorem ipsum, dolor sit amet consectetur adipisicing elit. In odit ratione hic saepe ab quas? Ullam voluptates cumque laboriosam magnam.</p>
      <p>Lorem ipsum, dolor sit amet consectetur adipisicing elit. Est hic atque quaerat reprehenderit mollitia earum id tempore quo, iusto sed laboriosam nam, expedita totam! Repudiandae.</p>
      <router-link to="/contact">
      <button class="info-btn">Контакти</button>
      </router-link>
    </div>

  </div>
</template>

<script>
export default {
  name: 'AboutView'
}
</script>

<style scoped>

.banner {
  height: 125px;
  background: url('../assets/banner.jpg');
  background-size: 1000px;
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

/* About main */

.heading {
  margin: 4rem 0;
  text-align: center;
  font-weight: 300;
}

.info-container {
  width: 55%;
  margin: 4rem auto;
}

/* Action btn */

.info-btn {
    text-align: center;
    margin: 1.5rem auto;
    cursor: pointer;
    padding: 0.5rem 2rem;
    color: #fff;
    background: #000;
    border: 1px solid #fff;
  }

  .info-btn:hover {
    padding: 0.5rem 2rem;
    color: #000;
    background: #fff;
    border: 1px solid #000;
    transition:  0.2s;
  }

  /* .info-btn:hover::after {
    transition: 0.6s;
    content: ' ->';
    color: #000;
  } */

@media only screen and (max-width: 600px) {
    .info-container {
      text-align: center;
      width: 80%;
    }
}

</style>