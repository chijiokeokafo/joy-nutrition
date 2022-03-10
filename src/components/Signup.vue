<template>
  <div class="find-the-joy-section">
      <div class="inner">
        <h1 class="margin-bottom-10">FIND THE JOY AGAIN</h1>
        <div class="input">
          <input type="text" placeholder="Email Address">
          <button class="green">Join</button>
        </div>
      </div>
    </div>
</template>

<style scoped lang="stylus">
  .find-the-joy-section
    background url('~@/assets/img/find-the-joy-bg.jpg') center center / cover no-repeat
    padding 100px 0
    text-align center
    position relative

    .inner
      width 68%
      max-width 1200px
      margin 0 auto

    h1
      color #F3F0E8
      position relative
      z-index 2

    .input input
      outline none
      border none
      background-color rgba(0, 0, 0, 0.4)
      padding 10px 20px
      box-sizing border-box
      height 40px
      color #F3F0E8
      font-family 'Montserrat', sans-serif
      width 60%
      max-width 600px
      margin-top 10px

      button
        background-color #F3F0E8
        color #B85459
</style>
