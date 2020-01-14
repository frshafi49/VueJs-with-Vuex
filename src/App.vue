<template>
  <div id="app">
    <product-list-one v-bind:products="products" />
    <product-list-two v-bind:products="products" />
  </div>
</template>

<script>
import ProductListOne from "./components/ProductListOne.vue";
import ProductListTwo from "./components/ProductListTwo.vue";

export default {
  name: "app",
  components: {
    ProductListOne,
    ProductListTwo
  },
  data() {
    return {
      products:[
        {name:'Banana Skin',price:20},
        {name:'Shiny Star',price:40},
        {name:'Green Shells',price:60},
        {name:'Red Shells',price:80},
      ]
    };
  }
};
</script>

<style>
body{
  font-family: Ubuntu;
  color:#555

}
</style>
