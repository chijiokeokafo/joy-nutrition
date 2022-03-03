<template>
  <div class="main-footer-container">
    <div class="inner-footer">
      <img src="@/assets/img/logo.png" alt="" class="footer-logo">
      <p>&copy;Joy Guthrie, RD<br>
      <a href="mailto:joyguthrierd@gmail.com">joyguthrierd@gmail.com</a><br>
      416-476-5491
      </p>
    </div>
  </div>
</template>

<style lang="stylus" scoped>
  .main-footer-container
    width 100%
    background-color #d0d197
    padding 30px

  .inner-footer
    padding 0 20px
    width 100%
    text-align center

  .footer-logo
    width 60px
    margin 0 auto 20px
    display block

  p
    font-size 12px
    letter-spacing 4px
    line-height 2

    a
      color inherit
      text-decoration none
      transition all 0.125s ease;

      &:hover
        color #fff
</style>
