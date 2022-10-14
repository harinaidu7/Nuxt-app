<template>
  <div>
    <Navbar/>
  </div>
</template>

<script>
import Home from "./Home.vue";
import Navbar from "./Navbar.vue";
export default {
    name: "IndexPage",
    components: { Home, Navbar }
};
</script>
