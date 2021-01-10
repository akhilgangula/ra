<template>
  <div id="products">
    <div class="wrapper">
      <div class="heading">Our Products</div>
      <div class="caption mt-3">Check what we have got!!</div>
      <div class="body mt-5">
        <div class="container-fluid content">
          <div class="row">
            <div class="col-lg col-md mt-3">
              <b-card title="Raw Magnesite Powder" :img-src="product1" img-alt="Image" img-top>
                <!-- <b-card-text>Processed from Raw Magnesite stones.</b-card-text> -->
              </b-card>
            </div>
            <div class="col-lg col-md mt-3">
              <b-card title="Gypsum Lumps" :img-src="product4" img-alt="Image" img-top>
                <!-- <b-card-text>Extracted in large, medium and small size Lumps.</b-card-text> -->
              </b-card>
            </div>
            <div class="col-lg col-md mt-3">
              <b-card title="Plaster of Paris" :img-src="product5" img-alt="Image" img-top>
                <!-- <b-card-text>Processed quick-setting gypsum plaster.</b-card-text> -->
              </b-card>
            </div>
          </div>
          <div class="row mt-md-5 mb-md-5">
            <div class="col-2"></div>
            <div class="col-lg-4 col-md-4 mt-3">
              <b-card title="Raw Magnesite Lumps" :img-src="product2" img-alt="Image" img-top>
                <!-- <b-card-text>Available is variety of sizes.</b-card-text> -->
              </b-card>
            </div>
            <div class="col-lg-4 col-md -4 mt-3">
              <b-card title="Gypsum Plaster" :img-src="product3" img-alt="Image" img-top>
                <!-- <b-card-text>Processed from fine gypsum Lumps.</b-card-text> -->
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