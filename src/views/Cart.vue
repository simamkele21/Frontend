<template>
  <!-- <Navbar /> -->
  <div class="cart">
    <img
      src="https://mdbcdn.b-cdn.net/img/new/standard/nature/184.webp"
      class="card-img-top"
      alt="Product img"
    />
    <div class="card-body">
      <h5 class="card-title">Card title</h5>
      <p class="card-text">product description</p>
      <p>Price</p>
      <a href="#!" class="btn btn-primary">Remove</a>
      <a href="#!" class="btn btn-primary">add item (+1)</a>
    </div>
  </div>
  <div class="Payment">
    <a href="#!" class="btn btn-primary">Cashout</a>
  </div>
</template>

<style>
.cart {
  width: 350px;
  padding: 0 auto;
  margin: 0 30px 0 30px;
  display: flex;
  flex-wrap: wrap;
}

.btn {
  padding: auto;
  space: evenly;
}
</style>

<script>
// import Navbar from "@/components/Navbar";

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
    fetch("https://complete-rest-api.herokuapp.com/api/cart")
      .then((res) => res.json())
      .then((json) => {
        console.log(product);
        this.product = json;
      })
      .catch((err) => console.log(err));
  },
};
</script>
