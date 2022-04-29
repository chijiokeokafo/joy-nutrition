<template>
  <div class="main-resources-container">
    <div class="resources-hero">
      <img src="@/assets/img/resources.svg" alt="">
    </div>
    <div class="resources-body">
      <div class="inner">
        <p>I’m here to help, but if you require immediate support, please call 911 or reach out to one of
        these outstanding networks:</p>
        <p>24-Hour Crisis Support: <a target="_blank" href="https://here247.ca/">https://here247.ca/</a> <a target="_blank" href="phone:1-844-437-3247">1-844-437-3247</a><br>
        Youth Help Line: <a target="_blank" href="#">519-745-9909</a><br>
        Women’s Crisis Services of Waterloo Region: <a target="_blank" href="https://wcswr.org/">https://wcswr.org/</a></p>

        <p>If you’re looking for broader information on nutrition counselling or eating disorder recovery,
        please check out the links below.</p>

        <p><strong>Organizations</strong><br>
        National Eating Disorder Information Centre (NEDIC) <a target="_blank" href="https://nedic.ca/">https://nedic.ca/</a><br>
        Health at Every Size ® <a target="_blank" href="https://haescommunity.com/">https://haescommunity.com/</a><br>
        Association for Size Diversity and Health <a target="_blank" href="https://asdah.org/">https://asdah.org/</a></p>

        <p><strong>Books, Websites and Podcasts</strong><br>
        Intuitive Eating: <a target="_blank" href="https://www.intuitiveeating.org/">https://www.intuitiveeating.org/</a><br>
        Dr. Michelle May and Mindful Eating: <a target="_blank" href="https://amihungry.com/">https://amihungry.com/</a><br>
        Food Pysch Podcast: <a target="_blank" href="https://christyharrison.com/foodpsych/">https://christyharrison.com/foodpsych/</a><br>
        The Bodylove Project Podcast: <a target="_blank" href="https://www.jessihaggerty.com/blppodcast/">https://www.jessihaggerty.com/blppodcast/</a></p>
      </div>
    </div>
    <Signup></Signup>
  </div>
</template>

<script>

import Signup from '@/components/Signup.vue'

export default {
  name: 'resources',
  components: {
    Signup
  }
}
</script>

<style lang="stylus" scoped>
  .main-resources-container
    padding-top 102px
    background-color #F3F0E8

  .resources-hero
    background url('~@/assets/img/about-hero.jpg') center center / cover no-repeat
    padding 80px 20px
    text-align center
    position relative

  .resources-body
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

  @media (max-width: 1000px)
    .main-resources-container
      padding-top 70px

    .resources-body
      padding 40px 0

      .inner
        padding 0
        width 80%

        p
          font-size 16px

          a
            overflow-wrap: break-word;

        .row
          flex-direction column

          .service-block
            width 100%
            margin-bottom 30px

</style>
