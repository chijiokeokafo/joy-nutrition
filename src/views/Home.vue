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

        <div class="dot-separator">
          <img style="width: 100%; margin: 60px 0 40px 0" src="@/assets/img/horizontal.png" alt="">
        </div>

        <div class="services-2-container">
          <div class="service-row row justify-start align-start">
            <img src="@/assets/img/eating-disorder-icon.svg" alt="">
            <div class="service-row-copy">
              <h2>EATING DISORDER RECOVERY</h2>
              <p>Recovery is possible! No matter where you are along the continuum of recovery, I will provide appropriate nutrition counselling to support your journey.</p>
              <button class="green">Learn More</button>
              <div class="dot-separator">
                <img style="width: 100%; margin: 60px 0 40px 0" src="@/assets/img/horizontal.png" alt="">
              </div>
            </div>
          </div>

          <div class="service-row row justify-start align-start">
            <img src="@/assets/img/disordered-icon.svg" alt="">
            <div class="service-row-copy">
              <h2>disordered eating/intuitive eating</h2>
              <p>Ready to break free of the yo-yo dieting cycle? As a qualifying Intuitive Eating Counselor, I will help you learn to listen to your body, to renew and better your relationship with food.</p>
              <button class="yellow">Learn More</button>
              <div class="dot-separator">
                <img style="width: 100%; margin: 60px 0 40px 0" src="@/assets/img/horizontal.png" alt="">
              </div>
            </div>
          </div>

          <div class="service-row row justify-start align-start">
            <img src="@/assets/img/general-nutrition-icon.svg" alt="">
            <div class="service-row-copy">
              <h2>general nutrition from a non-dieting approach</h2>
              <p>Each life stage brings different changes and challenges that can affect how you feel about food. I’m here to help.</p>
              <button class="red">Learn More</button>
              <div class="dot-separator">
                <img style="width: 100%; margin: 60px 0 40px 0" src="@/assets/img/horizontal.png" alt="">
              </div>
            </div>
          </div>
        </div>
      </div>
    </div>

    <div class="expect-section">
      <div class="inner">
        <h1 class="text-center">WHAT YOU CAN EXPECT</h1>

        <div class="expect-copy">
          <div class="first-section">
            <img src="@/assets/img/expect-icon.svg" alt="" style="">
            <p>Anyone I work with can expect utmost professionalism (though I’m known to swear when the
            situation calls for it!). But maybe more importantly, working with me is a collaboration. I don’t
            want my clients to feel like I’m just telling them what to do. Everything I do has a strong
            background of science-backed evidence, and I work hard to stay on top of new research and
            trends, to offer best-in-class support.</p>
          </div>
          <p>If you’re considering working with me, it’s important to know that I will push you to set goals
          and try things outside of your comfort zone, but I will not let you drown. We are a team, and I
          want you to succeed.</p>
          <p>My practice is also a safe space for everyone. You can expect a diverse, inclusive, judgment-free
          approach to your treatment.</p>
        </div>
        <button class="green block-center">Book an Appointment</button>
      </div>
    </div>

    <div class="find-the-joy-section">
      <div class="inner">
        <h1 class="margin-bottom-10">FIND THE JOY AGAIN</h1>
        <div class="input">
          <input type="text" placeholder="Email Address">
          <button class="green">Join</button>
        </div>
      </div>
    </div>
  </div>
</template>

<script>

export default {
  name: 'Home',
  components: {
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
    padding 100px 0 60px 0

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
    align-items flex-start

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

  .service-row img
    margin-right 50px

  .service-row-copy
    h2
      font-size 24px
      font-weight 700
      font-family 'Montserrat', sans-serif
      text-transform uppercase

    p
      margin-bottom 30px

  .expect-section
    background-color #F3F0E8
    padding 80px 0 60px 0

    .inner
      width 68%
      max-width 1200px
      margin 0 auto

    .expect-copy .first-section
      display flex
      flex-direction row
      justify-content space-between
      align-items center

      img
        margin-right 40px
        position relative
        top -30px

    .expect-copy p
      margin-bottom 30px

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
      margin-top 10px

      button
        background-color #F3F0E8
        color #B85459
</style>
