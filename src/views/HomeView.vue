<template>
  <div class="home">
    <!-- Banner -->
    <div class="banner">
      <div class="banner-text-container">
        <h1>Grow your business!</h1>
        <p>Grow your business with a beautifully crafted website</p>
        <button class="banner-btn">Повече Информация</button>
      </div>
    </div>

    <!-- Info section -->

    <!-- #1 -->

    <div class="info-section">
      <!-- Info box -->
      <div class="info-container">
        <p>about</p>
        <div>
          <h3>Lorem, ipsum dolor.</h3>
          <p>Lorem ipsum dolor, sit amet consectetur adipisicing elit. Sint, omnis aperiam obcaecati temporibus quidem iste neque aliquid magnam repellat delectus.</p>
          <button class="info-btn">Learn more</button>
        </div>
      </div>

      <!-- Img -->
      <div>
       <img src="../assets/logo.png" alt=""> 
      </div>  

    </div>

    <!-- #2 -->

    <div class="info-section">
      <!-- Img -->
      <div>
       <img src="../assets/logo.png" alt=""> 
      </div>

      <!-- Info box -->
      <div class="info-container">
        <p>about</p>
        <div>
          <h3>Lorem, ipsum dolor.</h3>
          <p>Lorem ipsum dolor, sit amet consectetur adipisicing elit. Sint, omnis aperiam obcaecati temporibus quidem iste neque aliquid magnam repellat delectus.</p>
          <button class="info-btn">Learn more</button>
        </div>
      </div>  

    </div>

    <!-- Services -->

    <div class="services-container">
      <h2 class="heading">Our Services</h2>
        <div class="servises-list">
          <!-- services cards -->
          <div class="servises-card">
            <span><i>Icon</i></span>
            <div>
              <h4>Support</h4>
              <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Iure, totam?</p>
            </div>
          </div>

          <div class="servises-card">
            <span><i>Icon</i></span>
            <div>
              <h4>Support</h4>
              <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Iure, totam?</p>
            </div>
          </div>

          <div class="servises-card">
            <span><i>Icon</i></span>
            <div>
              <h4>Support</h4>
              <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Iure, totam?</p>
            </div>
          </div>
      </div>

       <div class="servises-list">
          <!-- services cards -->
          <div class="servises-card">
            <span><i>Icon</i></span>
            <div>
              <h4>Support</h4>
              <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Iure, totam?</p>
            </div>
          </div>

          <div class="servises-card">
            <span><i>Icon</i></span>
            <div>
              <h4>Support</h4>
              <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Iure, totam?</p>
            </div>
          </div>

          <div class="servises-card">
            <span><i>Icon</i></span>
            <div>
              <h4>Support</h4>
              <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Iure, totam?</p>
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
  background: url('../assets/logo.png');
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
    border: 1px solid #000;
    transition:  0.2s;
  }

  .banner-btn:hover::after {
    transition: 0.6s;
    content: ' ->';
    color: #fff;
  }

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

  .info-btn:hover::after {
    transition: 0.6s;
    content: ' ->';
    color: #000;
  }

  /* Services */

  .services-container {
    margin-top: 4rem;
  }

  .heading {
    text-align: center;
  }

  .servises-list {
    margin-top: 2rem;
    display: flex;
    flex-direction: row;
    align-items: center;
    justify-content: space-around;
    flex-wrap: wrap;
  }

  .servises-card {
    width: 25%;
  }

  .servises-card div p{
    font-weight: 300;
  }

</style>