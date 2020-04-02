<template>
  <div>
    <Navbar />
    <div class="container mt-4">
      <Intro />
      <Package />
      <Feature />
      <Footer />
    </div>
  </div>
</template>

<script>
import Navbar from "./Navbar";
import Intro from "./Intro";
import Package from "./Package";
import Feature from "./Feature";
import Footer from "./Footer";

export default {
  components: {
    Navbar,
    Intro,
    Package,
    Feature,
    Footer
  }
};
</script>
