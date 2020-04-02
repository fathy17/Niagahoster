<template>
  <div class="navbar-container">
    <nav class="container navbar navbar-expand-lg navbar-light">
      <a class="navbar-brand" href="#">
        <img style="height:60px" src="../../assets/svg/niagahoster-logo.png" alt="logo" />
      </a>
      <button
        class="navbar-toggler"
        type="button"
        data-toggle="collapse"
        data-target="#navbarSupportedContent"
        aria-controls="navbarSupportedContent"
        aria-expanded="false"
        aria-label="Toggle navigation"
      >
        <span class="navbar-toggler-icon"></span>
      </button>

      <div class="collapse navbar-collapse" id="navbarSupportedContent">
        <ul class="navbar-nav ml-auto">
          <li class="nav-item" v-for="item in navItem" :key="item">
            <a class="nav-link" href="#">{{item}}</a>
          </li>
        </ul>
      </div>
    </nav>
  </div>
</template>

<script>
export default {
  name: "Navbar",
  data() {
    return {
      navItem: [
        "Hosting",
        "Domain",
        "Server",
        "Website",
        "Afiliasi",
        "Promo",
        "Pembayaran",
        "Review",
        "Kontak",
        "Blog"
      ]
    };
  }
};
</script>

<style>
</style>