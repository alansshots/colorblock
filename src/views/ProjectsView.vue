<template>
<div class="projects">
  <!-- Banner -->
     <div class="banner">
      <div class="banner-text-container">
        <h1>Приключени проекти</h1>
      </div>
    </div>

  <!-- Projects -->
  <ProjectsComponent/>
  
</div>
</template>

<script>
import ProjectsComponent from '../components/ProjectsComponent.vue'

export default {
   name:'ProjectsView',
   components: {
    ProjectsComponent,
  }
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

  /* Responsive */
  @media only screen and (max-width: 600px) {

    .banner-text-container h1 {
      font-size: 1.5rem;
    }

  }
</style>