<template>
  <!-- <div id="login-box">
    <div class="center">
      <h1>Sign up</h1>

      <input type="text" name="username" placeholder="Username" />
      <input type="text" name="email" placeholder="E-mail" />
      <input type="password" name="password" placeholder="Password" />
      <input type="password" name="password2" placeholder="Retype password" />

      <input type="submit" name="signup_submit" value="Sign me up" />
    </div>
  </div> -->
  <div class="row d-flex justify-content-center align-items-center h-100">
    <div class="col-12 col-md-8 col-lg-6 col-xl-5">
      <div class="card bg-dark text-white" style="border-radius: 1rem">
        <div class="card-body p-5 text-center">
          <div class="mb-md-5 mt-md-4 pb-5">
            <h2 class="fw-bold mb-2 text-uppercase">Sign-up</h2>
            <p class="text-white-50 mb-5">Please enter your Details!</p>

            <div class="form-outline form-white mb-4">
              <input
                type="username"
                id="typeUsernameX"
                class="form-control form-control-lg"
              />
              <label class="form-label" for="typeUsernameX">Username</label>
            </div>

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

            <div class="form-outline form-white mb-4">
              <input
                type="password"
                id="typePasswordX"
                class="form-control form-control-lg"
              />
              <label class="form-label" for="typePasswordX"
                >Retype Password</label
              >
            </div>

            <button class="btn btn-outline-light btn-lg px-5" type="submit">
              Sign Up
            </button>
          </div>

          <div>
            <p class="mb-0">
              Already have an account?
              <a href="#!" class="text-white-50 fw-bold"
                ><router-link :to="{ name: 'Login' }">Login </router-link></a
              >
            </p>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<style>
#login-box {
  position: relative;
  margin: 5% auto;
  width: 300px;
  height: 400px;
  background: #1d1d1d;
  border-radius: 2px;
  box-shadow: 0 2px 4px rgba(0, 0, 0, 0.4);
}

.center {
  position: absolute;
  top: 0;
  left: 0;
  box-sizing: border-box;
  padding: 40px;
  width: 300px;
  height: 400px;
}

h1 {
  margin: 0 0 20px 0;
  font-weight: 300;
  font-size: 28px;
}

input[type="text"],
input[type="password"] {
  display: block;
  box-sizing: border-box;
  margin-bottom: 20px;
  padding: 4px;
  width: 220px;
  height: 32px;
  border: none;
  border-bottom: 1px solid #aaa;
  font-family: "Roboto", sans-serif;
  font-weight: 400;
  font-size: 15px;
  transition: 0.2s ease;
}

input[type="text"]:focus,
input[type="password"]:focus {
  border-bottom: 2px solid #16a085;
  color: #16a085;
  transition: 0.2s ease;
}

input[type="submit"] {
  margin-top: 28px;
  width: 120px;
  height: 32px;
  background: #16a085;
  border: none;
  border-radius: 2px;
  color: #fff;
  font-family: "Roboto", sans-serif;
  font-weight: 500;
  text-transform: uppercase;
  transition: 0.1s ease;
  cursor: pointer;
}

input[type="submit"]:hover,
input[type="submit"]:focus {
  opacity: 0.8;
  box-shadow: 0 2px 4px rgba(0, 0, 0, 0.4);
  transition: 0.1s ease;
}

input[type="submit"]:active {
  opacity: 1;
  box-shadow: 0 1px 2px rgba(0, 0, 0, 0.4);
  transition: 0.1s ease;
}
</style>
