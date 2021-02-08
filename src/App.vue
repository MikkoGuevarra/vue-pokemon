<template>
  <div id="app">
    <img alt="Vue logo" src="https://images-na.ssl-images-amazon.com/images/I/619FF-ONnuL._AC_SY355_.jpg" />
    <!-- <HelloWorld msg="Welcome to Your Vue.js App" /> -->
    <CustomTitle />
    <Pokemons />
  </div>
</template>

<script>
// import HelloWorld from "./components/HelloWorld.vue";
import CustomTitle from "./components/CustomTitle.vue";
import Pokemons from "./pages/Pokemons.vue";

export default {
  name: "App",
  components: {
    // HelloWorld
    CustomTitle,
    Pokemons
},
};
</script>

<style lang="scss">
@import './assets/scss/app.scss';
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
