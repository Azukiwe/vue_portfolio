<template>
  <NavBar />
  <router-view />
  <Footer />
</template>

<script>
import NavBar from "@/components/NavBar.vue";
import Footer from "@/components/Footer.vue";

export default {
  components: { NavBar, Footer },
};
</script>
<style>
*,
*:before,
*:after {
  box-sizing: border-box;
  padding: 0;
  margin: 0;
}
NavBar, Footer{
  grid-column: 1/ -1;
} 
#app {
  font-family: "Courier New", Courier, monospace;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  background-color: lightgrey;
  
}

html {
  height: 100vh;
}

nav {
  padding: 30px;
}

nav a {
  font-weight: bold;
  color: #2c3e50;
}

nav a.router-link-exact-active {
  color: deeppink;
}
.title {
  position: relative;
  text-align: center;
  text-decoration: none;
  font-size: 2rem;
  font-weight: 600;
  margin-bottom: 60px;
  padding-top: 30px;
}
.title::before {
  content: "";
  position: absolute;
  bottom: 0px;
  left: 50%;
  width: 200px;
  height: 3px;
  background: black;
  transform: translateX(-50%);
}
.title::after {
  background-color: azure;
  position: absolute;
  bottom: -12px;
  left: 50%;
  transform: translateX(-50%);
}
.title::first-letter {
  font-size: 5rem;
  color: deeppink;
}


</style>
