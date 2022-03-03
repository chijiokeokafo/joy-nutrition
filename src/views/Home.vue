<template>
  <div class="home-container">
    <div class="hero-section">
      <div class="hero-copy">
        <h1>HELLO!</h1>
        <img src="@/assets/img/hero-so-glad.svg" alt="">
        <p>The very foundation of how we function, of how we move through the day, is food. Food is fuel,
        and we need it. But it’s so much more than that—nutrition is biology, yes, but it’s also culture, life, pleasure, fun. For some people, though, it’s scary. It translates to trauma. Punishment.</p>
        <p>We’re told day in and day out to change what we eat to change our bodies, to fit into a societal
        norm. When that message takes over, it can become toxic and all-consuming.</p>
        <p>Life is hard enough without having a negative relationship with food. That’s why I’m
        passionate about helping people learn to trust their bodies again, and to eat in a balanced,
        healthy way, to help them thrive. Food doesn’t need to be the cause of pain. It has the
        potential to instead become a basis for happiness, connection and joy.</p>
        <p style="margin-bottom: 30px;">Want to learn more? Read on for more about me and what I can do for you.</p>

        <div class="hero-cta-container">
          <button class="green">Learn More</button><button class="ghost">Get Started</button>
        </div>
      </div>

      <div class="hero-img">
        <img src="@/assets/img/hero-headshot.png" alt="">
      </div>
    </div>

    <!-- END HERO SECTION -->

    <div class="help-section">
      <div class="inner">
        <h1 class="text-center">HOW I CAN HELP</h1>

        <div class="help-copy">
          <div class="first-section">
            <img src="@/assets/img/help-icon.svg" alt="" style="">
            <p>I’ve been working as a registered dietitian in eating disorder recovery and treatment since
            2013. My clients have been all genders, ranged in age from adolescents to seniors, and have
            been at varying points of recovery. I strive to be a valued member of the
            multidisciplinary treatment teams of all of my clients.</p>
          </div>
          <p>In addition to eating disorder treatment, I have also worked with clients who have mood and
          anxiety disorders, women’s mental health concerns, exercise and movement issues,
          cardiovascular disease, pre-diabetes and diabetes, and challenges with perinatal nutrition.</p>
          <p>I provide nutrition counseling from a Healthy At Every Size (HAES) approach. My overall goal is
          to help you improve your relationship with food through science, and learning how to listen to your body beyond feelings of shame or guilt. In short, my focus is to help you understand and
          break through the nutrition “noise.”</p>
          <p style="font-weight: 600;"><strong>SERVICES:</strong></p>
        </div>

        <div class="services-container">

          <div class="service individual">
            <img src="@/assets/img/individual.svg" alt="">
            <p><strong>Individual Nutrition Counselling Services</strong>
            <br>Nutrition assessment and follow-up for eating disorder treatment (youth and adults), disordered eating, metabolic syndrome and more.</p>
          </div>

          <div class="dot-separator"><img src="@/assets/img/dots.png" alt=""></div>

          <div class="service group">
            <img src="@/assets/img/group.svg" alt="">
            <p><strong>Group Nutrition Presentations</strong>
            <br>Workshops on nutrition therapy for eating disorder treatment, disordered eating, nutrition and mental health.</p>
          </div>
        </div>
        <button class="red block-center">Learn More</button>

        <div>
          <img style="width: 100%; margin: 60px 0 40px 0" src="@/assets/img/horizontal.png" alt="">
        </div>
      </div>
    </div>
  </div>
</template>

<script>
// @ is an alias to /src
// import HelloWorld from '@/components/HelloWorld.vue'

export default {
  name: 'Home',
  components: {
    // HelloWorld
  }
}
</script>

<style lang="stylus" scoped>
  h1
    font-size 48px
    font-weight 700
    color #2A1C2D
    font-family 'Montserrat', sans-serif
    
  p
    font-size 16px
    font-weight 300
    color #2A1C2D
    font-family 'Montserrat', sans-serif

  .home-container
    padding-top 102px
    background-color #F3F0E8

  .hero-section
    background-color #F3F0E8
    padding 60px 0 0 0
    display flex
    flex-direction row
    justify-content center
    width 90%
    max-width 1200px
    margin 0 auto

    .hero-copy,
    .hero-img
      width 40%

    .hero-cta-container
      display flex
      flex-direction row
      justify-content flex-start
      align-items center

      

    .hero-img img
      display block

  .help-section
    background-color #f8f6f1
    padding-top 100px
    
    .inner
      width 68%
      max-width 1200px
      margin 0 auto
      
    .help-copy .first-section
      display flex
      flex-direction row 
      justify-content space-between
      align-items center
      
      img
        margin-right 40px
        position relative
        top -30px
        
    .help-copy p
      margin-bottom 30px
      
  .services-container
    display flex
    flex-direction row
    justify-content space-between
    align-items flex-end
    
    img
      margin-bottom 50px 
    
    .service
      width 46% 
      margin-bottom 50px
      
      img
        margin 0 auto 20px
        display block
      
  .dot-separator
    // height 100%
    // width 1px
    // border 1px dotted #333
      
  button
    color #F3F0E8
    font-size 16px
    font-weight 700
    font-family 'Montserrat', sans-serif
    padding 8px 20px
    margin-right 20px
    outline none
    cursor pointer
    transition all 0.25s ease
    
    &.green
      background-color #9CBCA5
      border 2px solid #9CBCA5
      
    &.red
      background-color #B85459
      border 2px solid #B85459
    
    &.yellow
      background-color #E8B67C
      border 2px solid #E8B67C

    &:hover
      background-color #fff
      border-color #fff
      color #9CBCA5

    &.ghost
      background-color transparent
      border 2px solid #9CBCA5
      color #9CBCA5

      &:hover
        background-color #fff
        border-color #fff
        color #9CBCA5
</style>
