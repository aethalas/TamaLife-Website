<template>
  <div id="app" class="max-width">
    <Header/>
  </div>
</template>

<script>
import Header from './components/Header.vue'

export default {
  name: 'app',
  components: {
    Header
  }
}
</script>

<style>
  @import url("https://fonts.googleapis.com/icon?family=Material+Icons");
  @import url("https://fonts.googleapis.com/css?family=Rubik");

  #app {
    font-family: 'Rubik', sans-serif;
    -webkit-font-smoothing: antialiased;
    -moz-osx-font-smoothing: grayscale;
    text-align: center;
    color: #2c3e50;
    margin-top: 60px;
    margin-bottom: 60px;
    font-size: 20px;
    box-shadow: 0 4px 8px 0 rgba(0, 0, 0, 0.2), 0 6px 20px 0 rgba(0, 0, 0, 0.19);
  }

  body {
    background: #ffffff;
    background-image: url("./assets/background.jpg");
    margin: 0;
  }

  .max-width {
    max-width: 1400px;
    margin: 0 auto;
  }

   @media (min-width: 1000px) and (max-width: 1400px) {
    .max-width {
      max-width: 85vw;
      margin: 0 auto;
      font-size: 1.4vw;
    }
   }

    @media (min-width: 1px) and (max-width: 999px) {
    #app {
      margin-top: 0px;
      margin-bottom: 0px;
      font-size: 9px;
    }

    .max-width {
      max-width: 100%;
      margin: 0 auto;
      font-size: 13px;
    }
   }
</style>
