<template>
  <div>
    <Nav />
    <!-- <transition name="pageFade" mode="out-in">
      <router-view/>
    </transition> -->
    <router-view v-slot="{ Component }">
      <transition name="pageFade" mode="out-in">
        <component :is="Component" />
      </transition>
    </router-view>

    <Footer />
  </div>
</template>

<script>
import Nav from '@/components/Nav.vue'
import Footer from '@/components/Footer.vue'

export default {
  components: {
    Nav,
    Footer
  }
}
</script>

<style>
  @import './assets/styles/main.css';
  @import './assets/styles/mobile.css';

  /*.pageFade-enter {
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
  }*/

  .pageFade-enter-active,
  .pageFade-leave-active { transition: opacity 0.3s ease; }

  .pageFade-enter-from,
  .pageFade-leave-to {
    opacity: 0;
  }

</style>
