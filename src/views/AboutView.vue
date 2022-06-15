<template>
  <div class="about">
    <!-- Banner -->
    <div class="banner">
      <div class="banner-text-container">
        <h1>Научете повече за нас!</h1>
      </div>
    </div>

    <!-- About main -->
    <h2 class="heading">Ние сме екип от креативни творци, които преосмислят онлайн пространството.</h2>

    <div class="info-container">
      <p>Colorblock е компания специализирана в изработката на уеб страници и лого дизайн.
Разполагаме с малък, но много креативен и изобретателен екип.</p>
      <p>Софтуерът далеч не е обикновен продукт. Той е съществена част от много бизнеси и като такъв той се нуждае от специално внимание за да покрие всички негови нужди. Colorblock е проект, посветен на създаването на уеб сайтове и софтуер, които се отличават.</p>
      <p> Colorblock е постоянно адаптираща се и иновативна компания готова да подпомогне развитието на вашия бизнес.</p>
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
  width: 70%;
  margin: 4rem auto 0 auto;
  text-align: center;
  font-weight: 300;
}

.info-container {
  width: 55%;
  margin: 3rem auto;
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

    .banner-text-container h1 {
      font-size: 1.4rem;
    }

    .heading {
      width: 90%;
      margin: 2rem auto 0 auto;
      font-size: 1.3rem;
    }

    .info-container {
      width: 90%;
      margin: 3rem auto;
    }
}

</style>