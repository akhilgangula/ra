<template>
  <section id="hero" >
    <div class="wrapper">
      <div class="align-middle title">RA Engineers</div>
      <div class="caption ">We import 
        <vue-typer 
        :text='["Gypsum", "Magnesite", "Plaster of Paris"]' 
        :repeat='Infinity'
        caret-animation='phase'
        erase-style='backspace'
        :erase-delay='50'
        ></vue-typer>
        </div>
    </div>
  </section>
</template>
<script>
import { VueTyper } from 'vue-typer'
export default {
  components: {
    VueTyper
  }
};
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
  font-size: calc(35px + (45 -35) * ((100vw - 300px) / (1600 - 300)));
}
.caption {
  font-size: calc(12px + (14 -12) * ((100vw - 300px) / (1600 - 300)));
}
</style>