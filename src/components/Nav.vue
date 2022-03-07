<template>
  <div class="main-nav-container navbar" :class="{ 'is-hidden': !showHeader }">
    <router-link to="/">
      <div class="logo">
        <img src="@/assets/img/logo-long.png" alt="">
      </div>
    </router-link>

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
      <h1>Book an Appointment</h1>
    </div>

  </div>
</template>

<script>
export default {
  name: 'Nav',
  data: () => ({
    showHeader: true,
    lastScrollPosition: 0,
    scrollOffset: 40
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

    h1
      font-size 18px
      font-weight 700
      color #F3F0E8
      font-family 'Montserrat', sans-serif

</style>
