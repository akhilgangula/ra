<template>
  <div id="header" class="position-fixed colored">
    <div>
      <b-navbar toggleable="lg">
        <b-navbar-brand class="m-3 logo">RA</b-navbar-brand>
        <b-navbar-toggle target="nav-collapse" class="border-0">
          <template v-slot:default="{ expanded }">
            <b-icon v-if="expanded" icon="list-nested"></b-icon>
            <b-icon v-else icon="list"></b-icon>
          </template>
        </b-navbar-toggle>
        <b-collapse id="nav-collapse" is-nav>
          <b-navbar-nav class="ml-auto">
            <b-navbar-nav>
              <b-nav-item class="pr-lg-5 p-3" v-scroll-to="'#hero'">
                <i class="fas fa-home mr-1"></i>Home
              </b-nav-item>
              <b-nav-item class="pr-lg-5 p-3 " v-scroll-to="{ el: '#abt-us',offset: -100 }">
                <i class="fab fa-autoprefixer mr-1"></i>About US
              </b-nav-item>
              <b-nav-item class="pr-lg-5 p-3" v-scroll-to="{ el: '#reach',offset: -100 }">
                <i class="fas fa-ship mr-1"></i>Reach
              </b-nav-item>
              <b-nav-item class="pr-lg-5 p-3" v-scroll-to="{ el: '#products' ,offset: -100}">
                <i class="fas fa-box m-1"></i>Products
              </b-nav-item>
              <b-nav-item class="pr-lg-5 p-3" v-scroll-to="{ el: '#contact' ,offset: -100}">
                <i class="fas fa-at mr-1"></i>Contact
              </b-nav-item>
            </b-navbar-nav>
          </b-navbar-nav>
        </b-collapse>
      </b-navbar>
    </div>
  </div>
</template>
<script>
import Vue from "vue";
import { NavbarPlugin } from "bootstrap-vue";
Vue.use(NavbarPlugin);
export default {};
</script>
<style scoped>
#header {
  z-index: 10;
  width: 100%;
}
.colored {
  background-color: white;
}
.logo {
  cursor:default;
}
</style>