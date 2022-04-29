<template>
  <div class="main-nav-container navbar" :class="{ 'is-hidden': !showHeader }">
    <router-link to="/">
      <div class="logo">
        <img src="@/assets/img/logo-long.png" alt="">
      </div>
    </router-link>

    <div class="show-hide">
      <div class="nav-links">
        <router-link to="/">
          <h1>Home</h1>
        </router-link>
        <span class="nav-pipe">|</span>
        <router-link to="/about">
          <h1>About</h1>
        </router-link>
        <span class="nav-pipe">|</span>
        <router-link to="/services">
          <h1>Services</h1>
        </router-link>
        <span class="nav-pipe">|</span>
        <router-link to="resources">
          <h1>Resources</h1>
        </router-link>
        <span class="nav-pipe">|</span>
        <router-link to="contact">
          <h1>Contact</h1>
        </router-link>
      </div>
      <div class="book-an-appt">
        <a target="_blank" style="" href="https://joynutrition.janeapp.com/">
          <h1>Book an Appointment</h1>
        </a>
      </div>
    </div>
    <div class="mobile-toggle" @click="toggleMobileNav()">
      <img src="@/assets/img/mobile2.png" alt="">
    </div>
    <transition name="pageFade" mode="in-out">
      <div class="mobile-links" v-if="isMobileNav" key="0">
        <router-link to="/" @click="this.isMobileNav = false">
          <h1>Home</h1>
        </router-link>
        <router-link to="/about" @click="this.isMobileNav = false">
          <h1>About</h1>
        </router-link>
        <router-link to="/services" @click="this.isMobileNav = false">
          <h1>Services</h1>
        </router-link>
        <router-link to="resources" @click="this.isMobileNav = false">
          <h1>Resources</h1>
        </router-link>
        <router-link to="contact" @click="this.isMobileNav = false">
          <h1>Contact</h1>
        </router-link>

        <a target="_blank" style="" href="https://joynutrition.janeapp.com/">
          <h1>Book an Appointment</h1>
        </a>
      </div>
    </transition>
  </div>
</template>

<script>
export default {
  name: 'Nav',
  data: () => ({
    showHeader: true,
    lastScrollPosition: 0,
    scrollOffset: 40,
    isMobileNav: false
  }),
  mounted () {
    this.lastScrollPosition = window.pageYOffset
    window.addEventListener('scroll', this.onScroll)
  },
  beforeUnmount () {
    window.removeEventListener('scroll', this.onScroll)
  },
  methods: {
    // Toggle if navigation is shown or hidden
    onScroll () {
      if (window.pageYOffset < 0) {
        return
      }
      if (Math.abs(window.pageYOffset - this.lastScrollPosition) < this.scrollOffset) {
        return
      }
      this.showHeader = window.pageYOffset < this.lastScrollPosition
      this.lastScrollPosition = window.pageYOffset
    },
    toggleMobileNav () {
      this.isMobileNav = !this.isMobileNav
    }
  }
}
</script>

<style lang="stylus" scoped>
  .main-nav-container
    display flex
    flex-direction row
    justify-content space-between
    align-items center
    position fixed
    background-color #F3F0E8
    width 100%
    box-shadow 0 14px 28px rgba(0,0,0,0.25), 0 10px 10px rgba(0,0,0,0.22)
    transform translateY(0)
    transition transform 300ms linear
    z-index 100

    &.is-hidden
      transform: translateY(-100%);

  .show-hide
    width calc( 100% - 100px )
    display flex
    align-self stretch

  .nav-links
    display flex
    flex-direction row
    justify-content flex-end
    align-items center
    margin-left auto
    margin-right 20px

    a
      text-decoration none
      position relative

      h1
        margin 0 10px
        font-size 16px
        font-family 'Montserrat', sans-serif
        font-weight 300
        color #2A1C2D

      &:after
        background none repeat scroll 0 0 transparent
        // bottom 0
        content ""
        display block
        height 2px
        left 50%
        position absolute
        background #9CBCA5
        transition width 0.3s ease 0s, left 0.3s ease 0s;
        width 0

      &:hover:after
        width 98%
        left 0

  .nav-pipe
    color #9CBCA5
    margin 0 10px
    font-size 16px
    font-family 'Montserrat', sans-serif
    font-weight 300

  .logo
    // max-height 70px
    width auto
    padding 16px
    box-sizing border-box

    img
      height 70px
      display block

  .book-an-appt
    background-color #B85459
    display flex
    justify-content center
    align-items center
    padding 2.5%
    box-sizing border-box
    align-self: stretch;

    a
      text-decoration none

    h1
      font-size 18px
      font-weight 700
      color #F3F0E8
      font-family 'Montserrat', sans-serif

  .mobile-toggle,
  .mobile-links
    display none

  .mobile-links
    position absolute
    top 74px
    left 0
    background-color #9cbca5
    padding 20px
    width 100%

  .show-enter-active,
  .show-leave-enter
    transform translateX(0)
    transition all .3s linear

  .show-enter,
  .show-leave-to
    transform translateX(100%)

  @media (max-width: 1200px)
    .logo img
      height 50px

  @media (max-width: 1000px)
    .logo
      padding 0

      img
        height 50px

    .main-nav-container
      padding 12px
      // position relative

    .nav-links,
    .book-an-appt
      display none

    .show-hide
      position absolute
      top 100px
      left -300px

    .mobile-toggle
      display block

      img
        width 35px

    .mobile-links
      display block
      // position absolute
      // top 74px
      // left 0
      // background-color #9cbca5
      // padding 20px
      // width 100%

      a
        text-decoration none

        h1
          font-size 20px
          font-weight 500
          color #f3f0e8

.menuFade-enter-active,
.menuFade-leave-active
  transition-duration 0.5s
  transition-property opacity
  transition-timing-function ease

.menuFade-enter,
.menuFade-leave-active
  opacity 0
</style>
