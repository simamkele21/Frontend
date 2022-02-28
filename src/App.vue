<template>
  <div id="nav">
    <Navbar />
  </div>
  <router-view />
</template>

<script>
import Navbar from "@/components/Navbar";

export default {
  name: "app",
  components: {
    Navbar,
  },
};
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
}

#nav {
  padding: 10px;
}

#nav a {
  font-weight: bold;
  color: #2c3e50;
}

#nav a.router-link-exact-active {
  color: #42b983;
}
body {
  background: #1d1d1d;
  color: #ffffff;
}
</style>
