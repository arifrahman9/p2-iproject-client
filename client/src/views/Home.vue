/* eslint-disable */ // eslint-disable-next-line //
<template>
  <div class="home">
    <!-- Start Jumbotron -->
    <div class="jumbotron">
      <div
        class="row d-flex justify-content-center align-items-center"
        style="height: 100vh"
      >
        <div class="col ms-3">
          <h1 class="text-dark pb-2">
            Website Cashier untuk Mencatat Transaksi Penjualan
          </h1>
          <button
            @click.prevent="toLogin"
            type="button"
            class="btn btn-lg mx-2 text-light"
            style="background-color: #301b3f"
          >
            Sign In
          </button>
          <button
            @click.prevent="toRegister"
            type="button"
            class="btn btn-lg mx-2 text-light"
            style="background-color: #301b3f"
          >
            Register
          </button>
        </div>
        <div class="col ilustrator">
          <img src="../img/undraw_around_the_world_re_n353.svg" />
        </div>
      </div>
    </div>
    <!-- End Jumbotron -->
  </div>
</template>

<script>
// @ is an alias to /src
export default {
  name: 'Home',
  methods: {
    toLogin() {
      this.$router.push('/login')
    },
    toRegister() {
      this.$router.push('/register')
    },
  },
}
</script>

<style>
.jumbotron {
  background-color: white;
  height: 100vh;
  overflow: hidden;
}
.ilustrator {
  height: 85%;
  width: 90%;
}
h4 {
  text-align: center;
}
</style>
