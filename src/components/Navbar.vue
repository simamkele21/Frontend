<template>
  <!-- <nav>
    <router-link :to="{ name: 'Products' }">Products </router-link> |
    <router-link :to="{ name: 'Cart' }">Cart </router-link>|
    <router-link :to="{ name: 'Profile' }">Profile </router-link> |
    <router-link :to="{ name: 'Login' }">Login </router-link> |
    <router-link :to="{ name: 'Home' }">Home </router-link>
  </nav> -->
  <!-- Navbar -->
  <nav class="navbar navbar-expand-lg navbar-light bg-light">
    <div class="container-fluid">
      <button
        class="navbar-toggler"
        type="button"
        data-mdb-toggle="collapse"
        data-mdb-target="#navbarSupportedContent"
        aria-controls="navbarSupportedContent"
        aria-expanded="false"
        aria-label="Toggle navigation"
      >
        <i class="fas fa-bars"></i>
      </button>

      <div class="collapse navbar-collapse" id="navbarSupportedContent">
        <a class="navbar-brand mt-2 mt-lg-0" href="#">
          <img
            src="https://i.postimg.cc/rsJxJQcB/Mr-J-s.png"
            height="45"
            alt="our Logo"
            loading="lazy"
          />
        </a>
        <ul class="navbar-nav me-auto mb-2 mb-lg-0">
          <li class="nav-item">
            <a class="nav-link"
              ><router-link :to="{ name: 'Home' }">Home </router-link></a
            >
          </li>
          <li class="nav-item">
            <a class="nav-link"
              ><router-link :to="{ name: 'Products' }"
                >Products
              </router-link></a
            >
          </li>
          <!-- <li class="nav-item">
            <a class="nav-link" href="#"
              ><router-link :to="{ name: 'Login' }">Login </router-link></a
            >
          </li> -->
          <!-- <li class="nav-item">
            <a class="nav-link" href="#"
              ><router-link :to="{ name: 'Contact' }">Contact </router-link></a
            >
          </li> -->
        </ul>
      </div>

      <div class="d-flex align-items-center">
        <a class="text-reset me-3" href="#">
          <router-link :to="{ name: 'Cart' }">Cart </router-link>
        </a>
        <div class="dropdown">
          <a
            class="dropdown-toggle d-flex align-items-center hidden-arrow"
            href="#"
            id="navbarDropdownMenuAvatar"
            role="button"
            data-mdb-toggle="dropdown"
            aria-expanded="false"
            ><router-link :to="{ name: 'Profile' }">Profile </router-link>
          </a>
          <ul
            class="dropdown-menu dropdown-menu-end"
            aria-labelledby="navbarDropdownMenuAvatar"
          >
            <li>
              <a class="dropdown-item" href="#">Logout</a>
            </li>
          </ul>
        </div>
      </div>
    </div>
  </nav>
</template>

<style>
#nav {
  /* background: #a4e7d9; */
  /* display: inline-block; */
  border-radius: 3px;
  padding: 5px;
  /* position: relative; */
}
</style>
