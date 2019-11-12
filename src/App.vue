<template>
  <div id="app">
    <Main/>
  </div>
</template>

<script>
import Main from './components/Main.vue'

export default {
  name: 'app',
  components: {
    Main
  }
}
</script>

<style>
  #app {
    font-size: 16px;
    -webkit-font-smoothing: antialiased;
    -moz-osx-font-smoothing: grayscale;
    text-align: center;
    padding: 0;
    margin: 0;
    color: #2c3e50;
  }
  .btn-success {
    background-color: #23A262;
    border-color: #23A262;
  }
  .green-text {
    color: #23A262;
  }
  @import url("https://fonts.googleapis.com/css?family=Montserrat:400,600,700,800,900&display=swap");

  body {
    font-family: "Montserrat", sans-serif !important;
  }
</style>
