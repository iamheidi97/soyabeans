<template>
  <div>
    <div class="main container mt-auto">
      <div class="col-md-12 left-border">
        <div class="col-md-12 left"></div>
      </div>
      <div class="col-md-12 left-Triangle-border float-left triangle-left-position">
        <div class="col-md-12 left-Triangle"></div>
      </div>
    </div>
  </div>
</template>
<script>
</script>
<style scoped>
.main {
  top: 0;
  position: relative;
  width: 100%;
  height: 200px;
  background-color: black;
}

.left-border {
  width: 99%;
  height: 49%;
  float: left;
  background: black;
  -webkit-clip-path: polygon(0 0, 0% 0, 100% 100%, 0 100%);
  clip-path: polygon(0 0, 100% 0, 100% 100%, 0 62%);
}
</style>
