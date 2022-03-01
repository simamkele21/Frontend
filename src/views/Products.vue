<template>
  <!-- <Navbar /> -->
  <div class="Products" v-if="products.length">
    <div v-for="products of products" :key="products.id" class="products">
      <img
        :src="products.img"
        :alt="products.title"
        style="width: 300px; height: 300px"
      />
      <div class="card-body">
        <h5 class="card-title">{{ products.title }}</h5>
        <p class="card-text">{{ products.description }}</p>
        <p>Price</p>
        <a href="#!" class="btn btn-primary">Add to Cart</a>
      </div>
    </div>
  </div>
  <div v-else>
    <p>Add products...</p>
  </div>
</template>

<style>
.cart {
  width: 350px;
  padding: 0 auto;
  margin: 0 50px 0 30px;
  display: flex;
  flex-wrap: wrap;
  color: #ffffff;
}

.mask {
  height: 350px;
}

.btn {
  padding: auto;
  space: evenly;
}
</style>

<script>
import Navbar from "@/components/Navbar";

export default {
  name: "app",
  // components: {
  //   Navbar,
  // },
  data() {
    return {
      products: null,
    };
  },
  mounted() {
    fetch("https://complete-rest-api.herokuapp.com/api/products")
      .then((res) => res.json())
      .then((json) => {
        console.log(product);
        this.product = json;
      })
      .catch((err) => console.log(err));
  },
};
</script>
