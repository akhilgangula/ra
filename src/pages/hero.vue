<template>
  <section id="hero" >
    <div class="wrapper">
      <div class="align-middle title">RA Engineers</div>
      <div class="caption ">We import Gypsum, Magnesite, Plaster of Paris</div>
    </div>
  </section>
</template>
<script>
export default {};
</script>
<style scoped>
#hero {
  background-repeat: no-repeat;
  display: table;
  width: 100%;
  height: 100vh;
  background: url("./../assets/world-map.gif") top center;
  background-size: cover;
}
.wrapper {
  display: table-cell;
  margin: 0;
  padding: 0;
  text-align: center;
  vertical-align: middle;
}
.title {
  font-size: calc(26px + (36 -26) * ((100vw - 300px) / (1600 - 300)));
}
.caption {
  font-size: calc(10px + (12 -10) * ((100vw - 300px) / (1600 - 300)));
}
</style>