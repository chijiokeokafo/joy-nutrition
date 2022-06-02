<template>
  <div class="main-services-container">
    <div class="services-hero">
      <img src="@/assets/img/services.svg" alt="">
    </div>

    <div class="services-body">
      <div class="col inner">
        <div class="row justify-between align-start">
          <div class="service-block">
            <img src="@/assets/img/service1.svg" alt="">
            <p><strong>15-Minute Consultation</strong></p>
            <p>FREE</p>
          </div>
          <div class="service-block">
            <img src="@/assets/img/service2.svg" alt="">
            <p><strong>Complete Nutrition Assessment</strong></p>
            <p>(90 mins + 30 mins preparation, coordination and documentation of care)<br>
            $150</p>
          </div>
          <div class="service-block">
            <img src="@/assets/img/service3.svg" alt="">
            <p><strong>Nutrition Follow-Up</strong></p>
            <p>(60 mins + 30 mins preparation, coordination and documentation of care)<br>
            $115</p>
          </div>
        </div>

        <p>Please check your extended health benefits package to see if you have coverage for appointments with a registered dietitian. Joy Nutrition does not do direct billing to insurance
        companies but will provide you with a receipt to submit for reimbursement. Registered
        dietitian services are a claimable healthcare expense. Fees are payable by email money transfer, all major credit cards, cash or cheque.</p>

        <p>If you’re interested in Group Nutrition Presentations, please reach out to discuss your needs
        and I’d be happy to provide a quote.</p>

        <div class="dot-separator" style="width: 100%;">
          <img style="width: 100%; margin: 60px 0 40px 0" src="@/assets/img/horizontal.png" alt="">
        </div>

        <h2 class="heading">LOCATION</h2>
        <p>Joy Nutrition is based in Kitchener, Ontario. Due to the COVID-19 pandemic, all appointments
        will be held virtually until further notice. An in-person location will be determined at a later
        date.</p>
      </div>
    </div>
    <Signup></Signup>
  </div>
</template>

<script>

import Signup from '@/components/Signup.vue'

export default {
  name: 'services',
  components: {
    Signup
  }
}
</script>

<style lang="stylus" scoped>
  .main-services-container
    padding-top 102px
    background-color #F3F0E8

  .services-hero
    background url('~@/assets/img/services-bg.jpg') center center / cover no-repeat
    padding 80px 20px
    text-align center
    position relative

  .services-body
    padding 90px 0

    img
      width 50%
      margin-right 40px

    .row.inner p
      width 50%

    .col.inner
      padding 60px 0 0

      p
        margin-bottom 30px

    ul
      list-style-type disc

      li
        font-size 16px
        font-weight 300
        color #2a1c2d
        font-family 'Montserrat', sans-serif
        margin-bottom 20px

  .service-block
    width 32%
    display flex
    flex-direction column
    align-items center
    justify-content flex-start
    text-align center

    img
      height 110px
      width auto !important
      margin 0 0 30px 0

    &:first-of-type img
      height 120px

    p
      margin-bottom 15px !important

      strong
        font-weight 700
        font-size 20px

  h2.heading
    font-size 45px
    font-weight 500
    font-family 'Montserrat', sans-serif
    text-align left
    width 100%
    margin-bottom 20px

  @media (max-width: 1000px)
    .main-services-container
      padding-top 70px

    .services-body .col.inner
      padding 0
      width 80%

      .row
        flex-direction column

        .service-block
          width 100%
          margin-bottom 30px
</style>
