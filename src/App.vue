<template>
  <div id="app" class="service theme colourway-miami">
    <!-- <img src="./assets/logo.png"> -->
    <!-- <router-view/> -->
    <Header/>
    <Footer/>
  </div>
</template>

<script>
import Header from './components/Header'
import Footer from './components/Footer'
export default {
  name: 'App',
  components: {
    Header,
    Footer,
  }
}
</script>

<style>
body {
  transition: opacity .4s ease;
  overflow-x: hidden;
}

body {
  margin: 0;
  font-size: 1rem;
  font-weight: 400;
  line-height: 1.5;
  color: #495057;
  text-align: left;
  background-color: #fff;
}

section {
  padding: 6rem 0;
}

section {
  position: relative;
}

#app {
  font-family: 'Karla', sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  /* padding-top: 60px; */
}

.bg-primary-3 {
  background-color:#010e1e!important;
}

.bg-primary-2 {
  background-color: #3423a6!important;
}




</style>
