<template>
  <!-- <Navbar /> -->
  <!-- <div class="cart">
    <div class="bg-image hover-overlay ripple" data-mdb-ripple-color="light">
      <img
        src="https://mdbcdn.b-cdn.net/img/new/standard/nature/111.webp"
        class="img-fluid"
      />
      <a href="#!">
        <div
          class="mask"
          style="background-color: rgba(251, 251, 251, 0.15)"
        ></div>
      </a>
    </div>
    <div class="cart-body">
      <h5 class="cart-title">Card title</h5>
      <p class="cart-text"></p>
      <p>Price</p>
      <a href="#!" class="btn btn-primary">Add to Cart</a>
    </div>
  </div> -->
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
      <a href="#!" class="btn btn-primary">Add to Cart</a>
    </div>
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
// import Navbar from "@/components/Navbar";

// export default {
//   name: "app",
//   components: {
//     Navbar,
//   },
// };
</script>
