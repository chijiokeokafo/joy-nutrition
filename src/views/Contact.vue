<template>
  <div class="main-contact-container">
    <div class="contact-hero">
      <img src="@/assets/img/contact.svg" alt="">
    </div>
    <div class="contact-body">
      <div class="inner row justify-start align-start">
        <div class="contact-form col justify-start align-start">
          <p>Reach out anytime. I'd be so happy to hear&nbsp;from&nbsp;you.</p>
          <form ref="form" @submit.prevent="sendEmail" style="text-align: right;">
            <input type="text" name="sender_name" class="name" placeholder="Full Name" v-model="name">
            <input type="email" name="sender_email" class="email" placeholder="Email" v-model="email">
            <textarea name="message" class="msg" placeholder="Message" v-model="message"></textarea>

            <transition name="pageFade" mode="out-in">
              <p v-if="isEmailSent">Thank you for reaching out, I'll be in touch soon!</p>
              <input v-else class="submit-btn" type="submit" value="SEND">
            </transition>
          </form>
        </div>
        <div class="contact-info">
          <p><strong>Joy Nutrition</strong></p>
          <p><a href="tel:416-476-5491">416 476 5491</a><br>
          <a href="mailto:joy@joynutrition.com">joy@joynutrition.com</a></p>
          <!-- <div class="row">
            <img src="@/assets/img/facebook.svg" alt="">
            <img src="@/assets/img/instagram.svg" alt="">
            <img src="@/assets/img/twitter.svg" alt="">
          </div> -->
        </div>
      </div>
    </div>
    <Signup></Signup>
  </div>
</template>

<script>

import Signup from '@/components/Signup.vue'
// import emailjs from 'emailjs-com'
import emailjs from '@emailjs/browser'

export default {
  name: 'contact',
  data () {
    return {
      name: '',
      email: '',
      message: '',
      isEmailSent: false
    }

    // SERVICE ID: service_x063vci
  },
  components: {
    Signup
  },
  methods: {
    sendEmail () {
      emailjs.sendForm('Joy-Nutrition', 'template_65609a7', this.$refs.form, 'oak8dZqZUI3qzfQXk')
        .then((result) => {
          console.log('SUCCESS!', result.text)

          this.name = ''
          this.email = ''
          this.message = ''
          this.isEmailSent = true
        }, (error) => {
          console.log('FAILED...', error.text)
        })
    }
  }
}
</script>

<style lang="stylus" scoped>
  .main-contact-container
    padding-top 102px
    background-color #F3F0E8

  .contact-hero
    background url('~@/assets/img/contact-bg.jpg') center center / cover no-repeat
    padding 80px 20px
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

  input.submit-btn
    color: #f3f0e8;
    font-size: 16px;
    font-weight: 700;
    font-family: 'Montserrat', sans-serif;
    padding: 8px 20px;
    margin-right: 0;
    outline: none;
    cursor: pointer;
    transition: all 0.25s ease;
    background-color: #b85459;
    border: 2px solid #b85459;
    width 200px

  @media (max-width: 1000px)
    .main-contact-container
      padding-top 70px

    .contact-body
      padding 40px 0

      .inner.row
        width 80%
        flex-direction column

        .contact-form
          width 100%
          margin 0 0 40px 0
</style>
