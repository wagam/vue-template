<template>
  <div class="navbar">
    <h1>{{ msg }}</h1>
    <h2>Login</h2>
  </div>
</template>

<script>
export default {
  name: "Navbar",
  props: {
    msg: String
  }
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
.navbar {
  position: relative;
  overflow: hidden;
  height: 200px;
  display: flex;
  justify-content: space-between;
  mix-blend-mode: difference;
  padding: 15px;
  &:before {
    content: "";
    position: absolute;
    width: 100%;
    height: 110%;
    top: 0;
    right: 75%;
    z-index: -1;
    -webkit-transform: rotate(30deg);
    background-color: #9966ff;
    border-bottom-right-radius: 30px;
    transform: rotate(30deg);
    transform-origin: top right;
  }
}

h1 {
  color: #42b983;
  mix-blend-mode: color-burn;
  margin-left: 100px;
}
ul {
  list-style-type: none;
  padding: 0;
}
li {
  display: inline-block;
  margin: 0 10px;
}
a {
  color: #42b983;
}
</style>