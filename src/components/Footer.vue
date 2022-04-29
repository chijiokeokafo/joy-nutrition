<template>
  <div class="main-footer-container">
    <div class="inner-footer row justify-between align-start">
      <div class="links text-left">
        <router-link to="/">
          <p><strong>Home</strong></p>
        </router-link>
        <router-link to="/about">
          <p><strong>About</strong></p>
        </router-link>
        <router-link to="/resources">
          <p><strong>Resources</strong></p>
        </router-link>
        <router-link to="/services">
          <p><strong>Service</strong></p>
        </router-link>
        <router-link to="/contact">
          <p><strong>Contact</strong></p>
        </router-link>
        <router-link to="/book">
          <p><strong>Book</strong></p>
        </router-link>
      </div>

      <!-- <div class="social col justify-between">
        <p><strong>Connect</strong></p>
        <img src="@/assets/img/facebook.svg" alt="">
        <img src="@/assets/img/instagram.svg" alt="">
        <img src="@/assets/img/twitter.svg" alt="">

      </div> -->
      <div class="contact text-left">
        <p><strong>Joy Nutrition</strong></p>
        <p>Joy Guthrie, RD</p>
        <p><a href="tel:416-476-5491">416 476 5491</a><br>
        <a href="mailto:joy@joynutrition.com">joy@joynutrition.health</a></p>
      </div>
    </div>
  </div>
</template>

<style lang="stylus" scoped>
  .main-footer-container
    width 100%
    background-color #F3F0E8
    padding 60px

  .inner-footer
    width 80%
    text-align center
    margin 0 auto

  .links a
    text-decoration none
    transition all 0.125s ease

    &:hover p
      color #9CBCA5

  p
    margin-bottom 10px
    transition all 0.125s ease

  .social
    img
      display block
      margin-bottom 20px

  .contact a
    color inherit
    text-decoration none
    transition all 0.25s ease

    &:hover
      color #9cbca5

  @media (max-width: 1000px)
    .inner-footer
      flex-flow row wrap
      width 100%

      .contact.text-left
        width 100%
        margin-top 40px
</style>
