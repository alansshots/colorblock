<template>
  <div id="app">
    <!-- Navbar -->
    <div class="navbar-container">
      <div class="logo-container">
        <router-link to="/">
          <img src="./assets/LogoColorblock.png" alt="logo">
        </router-link>
      </div>

    <div class="main-nav"> 
    <nav>
      <router-link to="/">Начало</router-link>
      <router-link to="/about">Информация</router-link>
      <router-link to="/projects">Проекти</router-link>
    </nav>
    </div>

    <div>
      <router-link to="/contact">
      <button class="nav-btn">Контакти</button>
      </router-link>
    </div>

    </div>

    <!-- Mobile navbar -->
    <div class="menu-mobile">
      <img src="./assets/LogoColorblock.png" alt="logo">
      <svg
      @click="isActive = !isActive"
      xmlns="http://www.w3.org/2000/svg" version="1.1" viewBox="0 0 16 16" width="25" height="25" fill="none" stroke="currentColor" stroke-linecap="round" stroke-linejoin="round" stroke-width="1.5"> 
      <path d="m2.75 12.25h10.5m-10.5-4h10.5m-10.5-4h10.5"/> </svg> 
    </div>

    <div class="navbar-mobile" v-if="isActive">
      <div> 
          <nav class="main-nav-mobile">

            <router-link to="/">
            <a @click="isActive = !isActive">Начало</a>
            </router-link>
            <router-link to="/about">
            <a @click="isActive = !isActive">Информация</a>
            </router-link>
            <router-link to="/contact">
            <a @click="isActive = !isActive">Контакти</a>
            </router-link>
            <!-- <router-link to="/projects">
            <a @click="isActive = !isActive">Контакти</a>
            </router-link> -->
          </nav>
      </div>
     </div>

    <!-- Load content -->
    <!-- <transition name="router-anim" enter-active-class="animated fadeIn" leave-active-class="animated fadeOut"> -->
      <router-view/>
    <!-- </transition> -->

    <!-- Footer -->
    <div  class="social-container">
      <a href="https://www.facebook.com/Colorblock-Web-Development-100395486057801" target="_blank" class="social-icon">
        <svg xmlns="http://www.w3.org/2000/svg" width="16" height="16" fill="currentColor" class="bi bi-facebook" viewBox="0 0 16 16">
        <path d="M16 8.049c0-4.446-3.582-8.05-8-8.05C3.58 0-.002 3.603-.002 8.05c0 4.017 2.926 7.347 6.75 7.951v-5.625h-2.03V8.05H6.75V6.275c0-2.017 1.195-3.131 3.022-3.131.876 0 1.791.157 1.791.157v1.98h-1.009c-.993 0-1.303.621-1.303 1.258v1.51h2.218l-.354 2.326H9.25V16c3.824-.604 6.75-3.934 6.75-7.951z"/>
        </svg>
      </a>
      <!-- <a href="" class="social-icon">
        <svg xmlns="http://www.w3.org/2000/svg" width="16" height="16" fill="currentColor" class="bi bi-instagram" viewBox="0 0 16 16">
        <path d="M8 0C5.829 0 5.556.01 4.703.048 3.85.088 3.269.222 2.76.42a3.917 3.917 0 0 0-1.417.923A3.927 3.927 0 0 0 .42 2.76C.222 3.268.087 3.85.048 4.7.01 5.555 0 5.827 0 8.001c0 2.172.01 2.444.048 3.297.04.852.174 1.433.372 1.942.205.526.478.972.923 1.417.444.445.89.719 1.416.923.51.198 1.09.333 1.942.372C5.555 15.99 5.827 16 8 16s2.444-.01 3.298-.048c.851-.04 1.434-.174 1.943-.372a3.916 3.916 0 0 0 1.416-.923c.445-.445.718-.891.923-1.417.197-.509.332-1.09.372-1.942C15.99 10.445 16 10.173 16 8s-.01-2.445-.048-3.299c-.04-.851-.175-1.433-.372-1.941a3.926 3.926 0 0 0-.923-1.417A3.911 3.911 0 0 0 13.24.42c-.51-.198-1.092-.333-1.943-.372C10.443.01 10.172 0 7.998 0h.003zm-.717 1.442h.718c2.136 0 2.389.007 3.232.046.78.035 1.204.166 1.486.275.373.145.64.319.92.599.28.28.453.546.598.92.11.281.24.705.275 1.485.039.843.047 1.096.047 3.231s-.008 2.389-.047 3.232c-.035.78-.166 1.203-.275 1.485a2.47 2.47 0 0 1-.599.919c-.28.28-.546.453-.92.598-.28.11-.704.24-1.485.276-.843.038-1.096.047-3.232.047s-2.39-.009-3.233-.047c-.78-.036-1.203-.166-1.485-.276a2.478 2.478 0 0 1-.92-.598 2.48 2.48 0 0 1-.6-.92c-.109-.281-.24-.705-.275-1.485-.038-.843-.046-1.096-.046-3.233 0-2.136.008-2.388.046-3.231.036-.78.166-1.204.276-1.486.145-.373.319-.64.599-.92.28-.28.546-.453.92-.598.282-.11.705-.24 1.485-.276.738-.034 1.024-.044 2.515-.045v.002zm4.988 1.328a.96.96 0 1 0 0 1.92.96.96 0 0 0 0-1.92zm-4.27 1.122a4.109 4.109 0 1 0 0 8.217 4.109 4.109 0 0 0 0-8.217zm0 1.441a2.667 2.667 0 1 1 0 5.334 2.667 2.667 0 0 1 0-5.334z"/>
        </svg>
      </a> -->
    </div>
    <div class="footer">
      <!-- <router-link to="/">Политика за поверителност</router-link> -->
      <p>Colorblock &copy; 2022 Всички права запазени. </p>
      <!-- <router-link to="/">Условия за ползване</router-link> -->
    </div>

  </div>
</template>

<script>

  export default {
    name:'App',
    data() {
      return {
        isActive: false,
      }
    }
  }
</script>
 

<style>
  @import "https://cdn.jsdelivr.net/npm/animate.css@3.5.1";
  @import url('https://fonts.googleapis.com/css2?family=Montserrat:ital,wght@0,300;0,400;0,500;0,600;0,700;0,800;1,300;1,400;1,500;1,600;1,700&display=swap');

  * {
    box-sizing: border-box;
    font-family: 'Montserrat', sans-serif;
  }

  body {
    margin: 0;
  } 

  .page {
    /* position: absolute; */
    width: inherit;
  }

  .navbar-container {
    width: 100%;
    display: flex;
    flex-direction: row;
    justify-content: space-around;
    align-items: center;
  }

  .logo-container img{
    width: 100px;
    margin: 1rem;
  }

  .menu-mobile img{
    width: 100px;
    margin: 0.7rem;
  }

  nav a {
   color: #000;
   text-decoration: none;
  }

  nav a.router-link-exact-active {
   border-bottom: 2px solid #000;
  } 

  .hidden {
    display: none;
  }

  .social-container a:visited { 
   text-decoration: none; 
   color: #4267B2; 
  }
    .menu-mobile {
      display: none;
    }

    .navbar-mobile {
      display: none;
    }

  @media only screen and (max-width: 600px) {
    .menu-mobile {
      display: block;
    }

    .navbar-mobile {
      display: block;
    }

    .navbar-container {
      display: none;
    }

    .navbar-mobile {
      height: 100%;
      background: #fff;
    }

    .menu-mobile {
      display: flex;
      flex-direction: row;
      justify-content: space-between;
      margin: 0 1rem;
      align-items: center;
    }

    .menu-mobile svg {
      cursor: pointer;
    }

    .main-nav-mobile {
      margin: 1rem 0;
      display: flex;
      flex-direction: column;
      justify-content: center;
      align-items: center;
    }

    .main-nav-mobile a{
      margin: 1rem 0;
    }
  }

  .main-nav nav {
    display: flex;
    flex-direction: row;
    justify-content: center;
    align-content: center;
  }

  .main-nav nav a {
    padding: 0rem 1.5rem;
  }

  .nav-btn {
    cursor: pointer;
    padding: 0.5rem 2rem;
    color: #fff;
    background: #000;
    border: 1px solid #000;
    transition:  0.4s;
  }

  .nav-btn:hover {
    padding: 0.5rem 2rem;
    color: #000;
    background: #fff;
    border: 1px solid #000;
    transition:  0.4s;
  }

  /* .nav-btn:hover::after {
    transition: 0.6s;
    content: '->';
  } */

  /* Footer */

  .social-container {
    border-top: dashed 2px #000;
    width: 100%;
    padding-top: 1rem;
    display: flex;
    flex-direction: row;
    justify-content: center;
    align-content: center;
  }

  .footer {
    display: flex;
    flex-direction: row;
    justify-content: space-around;
    align-content: center;
    text-decoration: none;
    text-align: center;
  }

  .footer a {
    text-decoration: none;  
    color: #000;
  }

  .footer a:hover {
    text-decoration: none;  
    scale: 0.9;
    transition: 0.4s;
  }

  .social-icon {
    padding: 0 1rem ;
    cursor: pointer;
  }

   .social-icon:hover {
    scale: 1.5;
    transition: ease-in-out 0.5s;
  }

  @media only screen and (max-width: 600px) {
    .footer a {
      display: none;
    }
  }
</style>
