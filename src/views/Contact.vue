<template>
  <div class="main-contact-container">
    <div class="contact-hero">
      <img src="@/assets/img/contact.svg" alt="">
    </div>
    <div class="contact-body">
      <div class="inner row justify-start align-start">
        <div class="contact-form col justify-start align-start">
          <input type="text" class="name" placeholder="Full Name">
          <input type="text" class="email" placeholder="Email">
          <textarea type="text" class="msg" placeholder="Message" />
          <button class="submit red">&nbsp;&nbsp;&nbsp;SEND&nbsp;&nbsp;&nbsp;</button>
        </div>
        <div class="contact-info">
          <p><strong>Joy Nutrition</strong></p>

          <p>123 Main Street, City, Ontario, Canada<br>
          ABC 123</p>
          <p>123 456 7890<br>
          email@domain.com</p>
          <div class="row">
            <img src="@/assets/img/facebook.svg" alt="">
            <img src="@/assets/img/instagram.svg" alt="">
            <img src="@/assets/img/twitter.svg" alt="">
          </div>
        </div>
      </div>
    </div>
    <Signup></Signup>
  </div>
</template>

<script>

import Signup from '@/components/Signup.vue'

export default {
  name: 'contact',
  components: {
    Signup
  }
}
</script>

<style lang="stylus" scoped>
  .main-contact-container
    padding-top 102px
    background-color #F3F0E8

  .contact-hero
    background url('~@/assets/img/contact-bg.jpg') center center / cover no-repeat
    padding 130px 0
    text-align center
    position relative

  .contact-body
    padding 90px 0

    p
      font-size 20px
      margin-bottom 20px

      strong
        font-weight 600

    a
      color #B85459
      text-decoration none
      transition all 0.125s ease

      &:hover
        color #9CBCA5

  .contact-form
    width 50%
    margin-right 30px

    input,
    textarea
      background-color #C4C4C4
      border none
      outline none
      color #F3F0E8
      padding 10px
      margin 0 20px 20px 0
      font-size 16px
      width 100%

    textarea
      min-height 200px
      resize none
      margin-bottom 30px

  .contact-info
    img
      margin-right 20px
</style>
