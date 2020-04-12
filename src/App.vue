<template>
  <div id="app">
    <ra-header />
    <hero />
    <about-us />
    <reach/>
    <product />
    <contact />
  </div>
</template>

<script>
import Hero from "@/pages/hero";
import RaHeader from "@/pages/header";
import AboutUs from "@/pages/aboutUs";
import Reach from "@/pages/reach";
import Product from "@/pages/product";
import Contact from "@/pages/contact";
export default {
  name: "App",
  components: {
    Hero,
    RaHeader,
    AboutUs,
    Reach,
    Product,
    Contact
  }
};
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  max-width: 100%;
}
</style>
