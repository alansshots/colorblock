<template>
  <div class="home">
    <!-- Banner -->
    <div class="banner">
      <div class="banner-text-container">
        <h1>Grow your business!</h1>
        <p>Grow your business with a beautifully crafted website!</p>
        <button class="banner-btn">Повече Информация</button>
      </div>
    </div>

    <!-- Info section -->

    <!-- #1 -->

    <div class="info-section">
      <!-- Info box -->
      <div class="info-container">
        <h6>информация</h6>
        <div>
          <h3>Lorem, ipsum dolor.</h3>
          <p>Lorem ipsum dolor, sit amet consectetur adipisicing elit. Sint, omnis aperiam obcaecati temporibus quidem iste neque aliquid magnam repellat delectus.</p>        
          <router-link to="/about">
          <button class="info-btn">Научете повече</button>
          </router-link>
        </div>
      </div>

      <!-- Img -->
      <div>
       <img src="../assets/logo.png" alt=""> 
      </div>  

    </div>

    <!-- #2 -->

    <div class="info-section reverse" >
      <!-- Img -->
      <div>
       <img src="../assets/logo.png" alt=""> 
      </div>

      <!-- Info box -->
      <div class="info-container">
        <h6>контакти</h6>
        <div>
          <h3>Lorem, ipsum dolor.</h3>
          <p>Lorem ipsum dolor, sit amet consectetur adipisicing elit. Sint, omnis aperiam obcaecati temporibus quidem iste neque aliquid magnam repellat delectus.</p>
          <!-- <button class="info-btn">Научете повече</button> -->
          <router-link to="/contact">
          <button class="info-btn">Контакти</button>
          </router-link>
        </div>
      </div>  

    </div>

    <!-- Services -->

    <div class="services-container">
      <h2 class="heading">Услуги</h2>
        <div class="servises-list">
          <!-- services cards -->
          <div class="servises-card">
            <span>
              <svg xmlns="http://www.w3.org/2000/svg" width="50" height="50" fill="currentColor" class="bi bi-wordpress" viewBox="0 0 16 16"> <path d="M12.633 7.653c0-.848-.305-1.435-.566-1.892l-.08-.13c-.317-.51-.594-.958-.594-1.48 0-.63.478-1.218 1.152-1.218.02 0 .039.002.058.003l.031.003A6.838 6.838 0 0 0 8 1.137 6.855 6.855 0 0 0 2.266 4.23c.16.005.313.009.442.009.717 0 1.828-.087 1.828-.087.37-.022.414.521.044.565 0 0-.371.044-.785.065l2.5 7.434 1.5-4.506-1.07-2.929c-.369-.022-.719-.065-.719-.065-.37-.022-.326-.588.043-.566 0 0 1.134.087 1.808.087.718 0 1.83-.087 1.83-.087.37-.022.413.522.043.566 0 0-.372.043-.785.065l2.48 7.377.684-2.287.054-.173c.27-.86.469-1.495.469-2.046zM1.137 8a6.864 6.864 0 0 0 3.868 6.176L1.73 5.206A6.837 6.837 0 0 0 1.137 8z"/> <path d="M6.061 14.583 8.121 8.6l2.109 5.78c.014.033.03.064.049.094a6.854 6.854 0 0 1-4.218.109zm7.96-9.876c.03.219.047.453.047.706 0 .696-.13 1.479-.522 2.458l-2.096 6.06a6.86 6.86 0 0 0 2.572-9.224z"/>
              <path fill-rule="evenodd" d="M0 8c0-4.411 3.589-8 8-8 4.41 0 8 3.589 8 8s-3.59 8-8 8c-4.411 0-8-3.589-8-8zm.367 0c0 4.209 3.424 7.633 7.633 7.633 4.208 0 7.632-3.424 7.632-7.633C15.632 3.79 12.208.367 8 .367 3.79.367.367 3.79.367 8z"/></svg>
            </span>
            <div>
              <h4>Wordpress и CMS</h4>
              <p>Разработване на уеб магазин или уеб страница чрез Wordpress или друг CMS.</p>
            </div>
          </div>

          <div class="servises-card">
            <span>
            <svg xmlns="http://www.w3.org/2000/svg" width="50" height="50" fill="currentColor" class="bi bi-code-slash" viewBox="0 0 16 16">
            <path d="M10.478 1.647a.5.5 0 1 0-.956-.294l-4 13a.5.5 0 0 0 .956.294l4-13zM4.854 4.146a.5.5 0 0 1 0 .708L1.707 8l3.147 3.146a.5.5 0 0 1-.708.708l-3.5-3.5a.5.5 0 0 1 0-.708l3.5-3.5a.5.5 0 0 1 .708 0zm6.292 0a.5.5 0 0 0 0 .708L14.293 8l-3.147 3.146a.5.5 0 0 0 .708.708l3.5-3.5a.5.5 0 0 0 0-.708l-3.5-3.5a.5.5 0 0 0-.708 0z"/></svg>  
            </span>
            <div>
              <h4>Уеб приложения и сайтове</h4>
              <p>Разработка на уеб приложение или уеб сайт от нулата.</p>
            </div>
          </div>
      </div>

       <div class="servises-list">
          <!-- services cards -->
          <div class="servises-card">
            <span>
              <svg xmlns="http://www.w3.org/2000/svg" width="50" height="50" viewBox="0 0 24 24"><path d="M16.24,11.51l1.57-1.57l-3.75-3.75l-1.57,1.57L8.35,3.63c-0.78-0.78-2.05-0.78-2.83,0l-1.9,1.9 c-0.78,0.78-0.78,2.05,0,2.83l4.13,4.13L3,17.25V21h3.75l4.76-4.76l4.13,4.13c0.95,0.95,2.23,0.6,2.83,0l1.9-1.9 c0.78-0.78,0.78-2.05,0-2.83L16.24,11.51z M9.18,11.07L5.04,6.94l1.89-1.9c0,0,0,0,0,0l1.27,1.27L7.02,7.5l1.41,1.41l1.19-1.19 l1.45,1.45L9.18,11.07z M17.06,18.96l-4.13-4.13l1.9-1.9l1.45,1.45l-1.19,1.19l1.41,1.41l1.19-1.19l1.27,1.27L17.06,18.96z"/>
              <path d="M20.71,7.04c0.39-0.39,0.39-1.02,0-1.41l-2.34-2.34c-0.47-0.47-1.12-0.29-1.41,0l-1.83,1.83l3.75,3.75L20.71,7.04z"/></svg>
            </span>
            <div>
              <h4>Лого дизайн</h4>
              <p>Изработване на модерно и съвременно лого за вашия бизнес.</p>
            </div>
          </div>

          <div class="servises-card">
            <span>
              <svg xmlns="http://www.w3.org/2000/svg" width="50" height="50" viewBox="0 0 24 24"><path d="M21,12.22C21,6.73,16.74,3,12,3c-4.69,0-9,3.65-9,9.28C2.4,12.62,2,13.26,2,14v2c0,1.1,0.9,2,2,2h1v-6.1 c0-3.87,3.13-7,7-7s7,3.13,7,7V19h-8v2h8c1.1,0,2-0.9,2-2v-1.22c0.59-0.31,1-0.92,1-1.64v-2.3C22,13.14,21.59,12.53,21,12.22z"/><circle cx="9" cy="13" r="1"/><circle cx="15" cy="13" r="1"/>
              <path d="M18,11.03C17.52,8.18,15.04,6,12.05,6c-3.03,0-6.29,2.51-6.03,6.45c2.47-1.01,4.33-3.21,4.86-5.89 C12.19,9.19,14.88,11,18,11.03z"/></svg>
            </span>
            <div>
              <h4>Поддръжка</h4>
              <p>Поддръжка на уеб магазини, сайтове и приложения.</p>
            </div>
          </div>
      </div>

    </div>

  </div>
</template>

<script>
export default {
  name: 'HomeView'
}
</script>

<style scoped>

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

.banner-btn {
    margin-top: 1.5rem;
    cursor: pointer;
    padding: 0.5rem 2rem;
    color: #000;
    background: #fff;
    border: 1px solid #fff;
  }

  .banner-btn:hover {
    padding: 0.5rem 2rem;
    color: #fff;
    background: #000;
    border: 1px solid #fff;
    transition:  0.4s;
  }

  /* .banner-btn:hover::after {
    transition: 0.6s;
    content: ' ->';
    color: #fff;
  } */

  /* Info section */
  .info-section {
    margin-top: 3rem;
    width: 100%;
    display: flex;
    flex-direction: row;
    justify-content: space-around;
    align-items: center;
  }
  
  .info-container {
    width: 40%;
  }

  .info-container h6 {
    margin: 0;
    font-size: 12px;
    font-weight: 300;
    text-transform: uppercase;
  }

  .info-btn {
    margin-top: 1.5rem;
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
    .info-section {
      margin-top: 3rem;
      width: 100%;
      display: flex;
      flex-direction: column;
      justify-content: space-around;
      align-items: center;
    }

    .reverse {
      flex-direction: column-reverse;
    }

    .info-container {
      width: 70%;
      text-align: center;
    }

  }

  /* Services */

  .services-container {
    margin-top: 4rem;
    margin-bottom: 4rem;
  }

  .heading {
    text-align: center;
  }

  .servises-list {
    width: 80%;
    margin: 2rem auto 0 auto;
    display: flex;
    flex-direction: row;
    align-items: center;
    justify-content: space-around;
    flex-wrap: wrap;
  }

  .servises-card {
    width: 33%;
  }

  .servises-card div p{
    font-weight: 300;
  }

  @media only screen and (max-width: 600px) {
    .servises-list {
      margin-top: 2rem;
      display: flex;
      flex-direction: column;
      justify-content: center;
      align-items: center;
      flex-wrap: wrap;
    }

    .servises-card {
      margin-top: 3rem;
      width: 70%;
      display: flex;
      flex-direction: column;
      justify-content: center;
      align-items: center;
    }

    .servises-card div {
      display: flex;
      flex-direction: column;
      justify-content: center;
      align-items: center;
      text-align: center;
    }

    .servises-card div p {
      margin: 0;
    }

  }

</style>