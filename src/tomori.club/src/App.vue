<template>
  <Nav />
  <router-view />
  <Footer />
</template>

<script>
import Nav from '@/components/Nav.vue';
import Footer from '@/components/Footer.vue';

export default {
  components: {
    Nav,
    Footer,
  },
}
</script>

<style>
body {
  background-image: url('./assets/background.png');
  background-position: center;
  background-size: 250px;
  background-repeat: repeat;
}
</style>
