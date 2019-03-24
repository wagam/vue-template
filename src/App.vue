<template>
  <div id="app">
    <Navbar msg="Brand name a little long"></Navbar>
    <Body/>
  </div>
</template>

<script>
import Body from "./components/Body.vue";
import Navbar from "./components/Navbar.vue";

export default {
  name: "app",
  components: {
    Body,
    Navbar
  }
};
</script>

<style lang="scss">
#app {
  font-family: "Avenir", Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
}

body {
  background-color: #fcfcfc
}

body, h1, h2, h3 {
  margin: 0;
}
</style>
