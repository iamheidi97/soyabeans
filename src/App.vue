<template>
  <div id="app">
    <Main />
  </div>
</template>

<script>
import Main from "./components/Main.vue";

export default {
  name: "app",
  components: {
    Main
  }
};
</script>

<style>
#app {
  font-size: 16px;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  box-sizing: border-box;
  overflow: hidden;
  padding: 0;
  margin: 0;
  color: #2c3e50;
}
.btn-success {
  background-color: #23a262;
  border-color: #23a262;
}
.green-text {
  color: #23a262;
}
@import url("https://fonts.googleapis.com/css?family=Montserrat:400,600,700,800,900&display=swap");

body {
  font-family: "Montserrat", sans-serif !important;
}

  @media (max-width: 576px) {
      .display-4 {
        font-size: 2.8rem;
      }
  }

  /* // Medium devices (tablets, 768px and up) */
  @media (max-width: 768px) {  }

  /* // Large devices (desktops, 992px and up) */
  @media (min-width: 992px) {  }

  /* // Extra large devices (large desktops, 1200px and up) */
  @media (min-width: 1200px) { }

</style>
