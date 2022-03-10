<template>
  <div class="main-contact-container">
    <div class="contact-hero">
      <img src="@/assets/img/contact.svg" alt="">
    </div>
    <div class="contact-body">
      <div class="inner">
        CONTACT FORM GOES HERE
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

</style>
