<template>
  <!-- <Navbar /> -->
  <div class="container">
    <div class="prow">
      <div class="col-4">
        <div class="profile-img">
          <i class="far fa-user-circle"></i>
        </div>
        <br />
        Since 9 + 4 = 13 &gt; 12, this 4-column-wide div gets wrapped onto a new
        line as one contiguous unit.
      </div>
      <div class="col-6">
        .col-6<br />Subsequent columns continue along the new line.
      </div>
    </div>
  </div>
</template>

<script>
// import Navbar from "@/components/Navbar";

// export default {
//   name: "app",
//   components: {
//     Navbar,
//   },
// };
</script>

<style>
.prow {
  background-color: white;
  border-radius: 9px;
  /* height: 500px; */
  width: 150vh;
}
.profile-img {
  height: 50px;
  width: 20vh;
}
</style>
