<template>
  <!-- <div class="home">
    <h1>Great day orders</h1>

    <MDBBtn color="white" target="_blank" rel="noopener">
      <router-link :to="{ name: 'Login' }">Login </router-link></MDBBtn
    >
  </div> -->

  <!-- Jumbotron -->
  <div
    class="bg-image p-5 text-center shadow-1-strong rounded mb-5 text-white"
    style="
      background-image: url('https://i.postimg.cc/GpT3rQ7v/2de6e3104339325-5f60e46d264dc.jpg');
    "
  >
    <h1 class="mb-3 h1">MR J's</h1>
    <h3>Munch Aways</h3>

    <MDBBtn color="white" target="_blank" rel="noopener">
      <router-link :to="{ name: 'Login' }">Login </router-link></MDBBtn
    >
  </div>
  <!-- Jumbotron -->
</template>

<script>
import {
  MDBModal,
  MDBModalHeader,
  MDBModalTitle,
  MDBModalBody,
  MDBModalFooter,
  MDBBtn,
  MDBRow,
  MDBInput,
  MDBCheckbox,
  MDBCol,
} from "mdb-vue-ui-kit";
import { ref } from "vue";

export default {
  components: {
    MDBModal,
    MDBModalHeader,
    MDBModalTitle,
    MDBModalBody,
    MDBModalFooter,
    MDBBtn,
    MDBRow,
    MDBCol,
    MDBInput,
    MDBCheckbox,
  },
  setup() {
    const exampleSideModal1 = ref(false);
    return {
      exampleSideModal1,
    };
    const checkForm = (e) => {
      e.target.classList.add("was-validated");
    };
    const input1 = ref("Mark");
    const input2 = ref("Otto");
    const input3 = ref("");
    const input4 = ref("");
    const checkbox1 = ref(false);
    return {
      input1,
      input2,
      input3,
      input4,
      checkbox1,
      checkForm,
    };
  },
};
</script>

<style>
h1 {
  padding-top: 250px;
}
.bg-image {
  height: 88vh;
}
</style>
