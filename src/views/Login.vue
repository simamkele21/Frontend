<template>
  <div class="row d-flex justify-content-center align-items-center h-100">
    <div class="col-12 col-md-8 col-lg-6 col-xl-5">
      <div class="card bg-dark text-white" style="border-radius: 1rem">
        <div class="card-body p-5 text-center">
          <div class="mb-md-5 mt-md-4 pb-2">
            <h2 class="fw-bold mb-2 text-uppercase">Login</h2>
            <p class="text-white-50 mb-5">
              Please enter your login and password!
            </p>
            <div class="form-outline form-white mb-4">
              <input
                type="email"
                id="typeEmailX"
                class="form-control form-control-lg"
              />
              <label class="form-label" for="typeEmailX">Email</label>
            </div>
            <div class="form-outline form-white mb-4">
              <input
                type="password"
                id="typePasswordX"
                class="form-control form-control-lg"
              />
              <label class="form-label" for="typePasswordX">Password</label>
            </div>
            <button class="btn btn-outline-light btn-lg px-5" type="submit">
              <router-link :to="{ name: 'Profile' }">Login </router-link>
            </button>
          </div>
          <div>
            <p class="mb-0">
              Don't have an account?
              <a href="#!" class="text-white-50 fw-bold"
                ><router-link :to="{ name: 'Signup' }">Signup </router-link></a
              >
            </p>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<style>
.gradient-custom {
  background: #1d1d1d;
}
.row {
  padding-top: 50px;
}
</style>

<script>
export default {
  mounted() {
    fetch("https://complete-rest-api.herokuapp.com/api/user")
      .then((res) => res.json())
      .then((json) => {
        this.user = data;
        console.log(user);
      })
      .catch((err) => console.log(err));
  },
};
</script>
