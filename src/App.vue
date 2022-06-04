<template>
  <div id="app">
    <!-- Navbar -->
    <div class="navbar-container">
      <div>
        <h2>Colorblock</h2>
      </div>

    <div class="main-nav"> 
    <nav>
      <router-link to="/">Начало</router-link>
      <router-link to="/about">Информация</router-link>
      <router-link to="/projects">Проекти</router-link>
    </nav>
    </div>

    <div>
      <button>Контакти</button>
    </div>

    </div>

    <!-- Load content -->
    <router-view/>

    <!-- Footer -->
  </div>
</template>

<style>
  @import url('https://fonts.googleapis.com/css2?family=Comfortaa:wght@300;400;500;600;700&display=swap');

  * {
    font-family: 'Comfortaa', cursive;
  }

  .navbar-container {
    width: 100%;
    display: flex;
    flex-direction: row;
    justify-content: space-around;
    align-items: center;
  }

  .main-nav nav {
    display: flex;
    flex-direction: row;
    justify-content: center;
    align-content: center;
  }

  .main-nav nav a {
    padding: 0rem 1rem;
  }



/* #app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
}

nav {
  padding: 30px;
}

nav a {
  font-weight: bold;
  color: #2c3e50;
}

nav a.router-link-exact-active {
  color: #42b983;
} */
</style>
