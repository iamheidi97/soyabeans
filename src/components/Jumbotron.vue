<template>
  <div class="my-jumbo">
    <div class="col-8 p-0 ml-auto mr-4 text-left">
      <b-jumbotron>
        <label>Be Japan-ready in a month!</label>
      </b-jumbotron>
    </div>
  </div>
</template>
<script>
</script>
<style scoped>
@import url('https://fonts.googleapis.com/css?family=Montserrat:900&display=swap');

.my-jumbo{
    font-family: 'Montserrat', sans-serif;
    top: 30%;
    right: 0;
    position: absolute;
    z-index: 200;
    height: 100vh;
}
.jumbotron{
    width: 100%;
    font-family: inherit;
    color: #fff9ba;
    background-color: transparent;
    font-weight: bold;
}
label{
    font-size: 3.5rem;
    /* text-shadow: px 1px 0px #4f9e37; */
    text-shadow: 4px 4px 0px #4f9e37;
}
</style>
