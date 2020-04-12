<template>
  <div id="products">
    <div class="wrapper">
      <div class="heading">Our Products</div>
      <div class="caption mt-3">Here is what we got</div>
      <div class="body mt-5">
        <div class="container-fluid content">
          <div class="row">
            <div class="col-lg col-md mt-3">
              <b-card title="Title" :img-src="product1" img-alt="Image" img-top>
                <b-card-text>This card has supporting text below as a natural lead-in to additional content.</b-card-text>
              </b-card>
            </div>
            <div class="col-lg col-md mt-3">
              <b-card title="Title" :img-src="product4" img-alt="Image" img-top>
                <b-card-text>This card has supporting text below as a natural lead-in to additional content.</b-card-text>
              </b-card>
            </div>
            <div class="col-lg col-md mt-3">
              <b-card title="Title" :img-src="product5" img-alt="Image" img-top>
                <b-card-text>This card has supporting text below as a natural lead-in to additional content.</b-card-text>
              </b-card>
            </div>
          </div>
          <div class="row mt-md-5 mb-md-5">
            <div class="col-2"></div>
            <div class="col-lg-4 col-md-4 mt-3">
              <b-card title="Title" :img-src="product2" img-alt="Image" img-top>
                <b-card-text>This card has supporting text below as a natural lead-in to additional content.</b-card-text>
              </b-card>
            </div>
            <div class="col-lg-4 col-md -4 mt-3">
              <b-card title="Title" :img-src="product3" img-alt="Image" img-top>
                <b-card-text>This card has supporting text below as a natural lead-in to additional content.</b-card-text>
              </b-card>
            </div>
            <div class="col-2"></div>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
import product1 from "@/assets/products/product-1.jpg";
import product2 from "@/assets/products/product-2.jpeg";
import product3 from "@/assets/products/product-3.jpeg";
import product4 from "@/assets/products/product-4.jpeg";
import product5 from "@/assets/products/product-5.jpeg";

export default {
  data() {
    return {
      product1,
      product2,
      product3,
      product4,
      product5
    };
  }
};
</script>

<style scoped>
.heading {
  font-size: calc(22px + (26 -22) * ((100vw - 300px) / (1600 - 300)));
  font-weight: bold;
}
.content {
  width: 80%;
}
</style>