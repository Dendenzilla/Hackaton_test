<template>
  <div id="app">
    <Header/>
    <div id="nav">
      <!-- <router-link to="/">Home</router-link>| -->
      <!-- <router-link to="/about">About</router-link> -->
    </div>
    <router-view/>
    <Footer/>
  </div>
</template>
<script>
import Header from "./components/Header.vue";
import Footer from "./components/Footer.vue";
export default {
  name: "app",
  components: {
    Header,
    Footer
  }
};



</script>
<style lang="scss">
@import url('https://fonts.googleapis.com/css?family=Roboto:500,700|Open+Sans:400,600');
@import url('https://use.fontawesome.com/releases/v5.7.2/css/all.css');
@import url('~@/assets/style.min.css');
#app {
  text-align: center;
  font-family: 'Open Sans', sans-serif;
  margin: 0;
}
body{
  margin: 0;
}
</style>
