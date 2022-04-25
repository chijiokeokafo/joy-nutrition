<template>
  <div class="main-about-container">
    <div class="about-hero">
      <img src="@/assets/img/about-hero.svg" alt="">
    </div>

    <div class="about-body">
      <div class="row inner justify">
        <img src="@/assets/img/about-headshot.png" alt="">
        <p>I landed in this space by way of my education. I had intended to study medicine, so I started with a major in Kinesiology. But then, during my undergrad degree, I took a nutrition and physiology course and I was mesmerized. I’m a big science nerd and I fell in love with the science behind nutrition. I found it particularly interesting that our bodies really are largely shaped by genetics and metabolic pathways—and that this is the opposite of the Western message that you can change your body by changing what you put into it. I also love how culture, religion, social determinants of health, education and more intersect with nutrition. This is where you get to know people, and it’s one of the aspects I love most about my work. So, long story short, I finished my degree and changed my path to nutrition.</p>
      </div>
      <div class="col inner">
        <p>This decision has turned out to be one of the most impactful and meaningful of my life. The
        work is both challenging and gratifying, and when I’m able to help a client, it reaffirms my
        choice. This work isn’t just about food; it’s also about the role mental health plays in our
        relationship with nutrition. Helping people to understand this and factor it into their recovery is
        important and, for me, very fulfilling.</p>

        <p>In addition to my passion for the nutrition field, I’m also proud to be a woman of colour in this
        space. The perspectives of people of colour are rarely reflected in nutrition education and
        professional practice, and this needs to change. The call to diversify dietetics will hopefully
        mean that one day everyone will be able to find a professional who represents them, who looks
        like them, and who can tailor their discussions and treatment to reflect different experiences.</p>

        <p>Outside of my work life, I am a busy wife and mom to two little ones. I love to travel near and
        far, have family meals, dance in my kitchen and crochet Amigurumi. Growing up on the east
        coast, being near the water will forever be my happy place.</p>
      </div>
    </div>

    <div class="education-hero">
      <img src="@/assets/img/education.svg" alt="">
    </div>

    <div class="about-body">
      <div class="inner education-inner">
        <ul>
          <!-- <li>Registered Dietitian with the College of Dietitians of Ontario (2013)</li>
          <li>RD working in Outpatient Eating Disorder Treatment and Mood &amp; Anxiety Treatment
          programs since 2013 (St. Joseph’s Healthcare Hamilton, Stratford General Hospital,
          CMHA – Waterloo/Wellington)</li>
          <li>Certified Intuitive Eating Counselor (In Progress)</li>
          <li>Certified Exercise Physiologist – Canadian Society for Exercise Physiology (2007)</li>
          <li>Principles of CBT for Psychosis (2020)</li>
          <li>Principles of Family-Based Treatment for Adolescent Eating Disorders (2019)</li>
          <li>Introduction to Group-Based Dialectical Behaviour Therapy (2019)</li>
          <li>Intro to Cognitive Behavioral Therapy Level 2 – McMaster University (2017)</li>
          <li>Intro to Cognitive Behavioral Therapy Level 1 – McMaster University (2014)</li>
          <li>Honours BASc Nutrition and Food – Ryerson University (2011)</li>
          <li>Honours BSc Human Kinetics – University of Ottawa (2007)</li> -->
          <li>Registered Dietitian with the College of Dietitians of Ontario (2013)</li>
          <li>Certified Exercise Physiologist – Canadian Society for Exercise Physiology (2007)</li>
          <li>Certified Intuitive Eating Counselor (In Progress)</li>
          <li>Principles of Family-Based Treatment for Adolescent Eating Disorders (2019)</li>
          <li>Intro to Cognitive Behavioral Therapy Level 1 & 2 – McMaster University</li>
        </ul>
      </div>
    </div>
    <Signup></Signup>
  </div>
</template>

<script>

import Signup from '@/components/Signup.vue'

export default {
  name: 'About',
  components: {
    Signup
  }
}
</script>

<style lang="stylus" scoped>
  .main-about-container
    padding-top 102px
    background-color #F3F0E8

  .about-hero
    background url('~@/assets/img/about-hero.jpg') center center / cover no-repeat
    padding 130px 0
    text-align center
    position relative

  .about-body
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

  .education-hero
    background url('~@/assets/img/education-bg.jpg') center center / cover no-repeat
    padding 130px 0
    text-align center
    position relative

  .education-inner
    max-width 900px

  @media (max-width: 1000px)
    .main-about-container
      padding-top 0

    .about-body
      padding 40px 0

      .row.inner
        flex-direction column !important
        width 70%

        img
          margin 0 auto
          width 100%

        p
          width 100%

    .education-hero
      padding 80px 30px

</style>
