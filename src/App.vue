<template>
  <div>
    <!-- <VueFixedHeader> -->
      <Nav />
    <!-- </VueFixedHeader> -->
    <transition name="pageFade" mode="out-in">
      <router-view/>
    </transition>
    <Footer />
  </div>
</template>

<script>
// import VueFixedHeader from 'vue-fixed-header'
import Nav from '@/components/Nav.vue'
import Footer from '@/components/Footer.vue'

export default {
  components: {
    Nav,
    Footer
    // VueFixedHeader
  }
}
</script>

<style>
  @import './assets/styles/main.css';

  .pageFade-enter {
      opacity: 0;
  }

  .pageFade-enter-active {
      transition: opacity .3s ease;
  }

  .pageFade-leave {
    opacity: 1;
  }

  .pageFade-leave-active {
      transition: opacity .3s ease;
      opacity: 0;
  }

  .navbar.vue-fixed-header--isFixed {
    position: fixed;
    left: 0;
    top: 0;
    width: 100vw;
  }
</style>
