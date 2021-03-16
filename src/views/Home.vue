<template>
  <div class="home">
    <!-- <HelloWorld msg="Welcome to Your Vue.js App" /> -->
    <NavBar></NavBar>
  </div>
</template>

<script>
import NavBar from "@/components/NavBar.vue";
// @ is an alias to /src

export default {
  name: "Home",
  components: {
    NavBar
  }
};
</script>
<style media="screen">
.home {
  height: 100vh;
  /* background-color: #262c47; */
  background: #6441a5; /* fallback for old browsers */
  background: -webkit-linear-gradient(
    to bottom,
    #2a0845,
    #6441a5
  ); /* Chrome 10-25, Safari 5.1-6 */
  background: linear-gradient(
    to bottom,
    #2a0845,
    #6441a5
  ); /* W3C, IE 10+/ Edge, Firefox 16+, Chrome 26+, Opera 12+, Safari 7+ */
}
</style>
