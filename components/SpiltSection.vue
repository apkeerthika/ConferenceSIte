<template lang="pug">
section.spilt-section
  .container
    h2 WHAT TO EXPECT FROM INBOUND 2019
    .expectation(v-for="(s, i) in spiltSections", :key="i")
      .header-text(v-html="s.content")
</template>

<script>
export default {
  data () {
    return {
      spiltSections: [
        {
          content: '<h5>INSPIRING KEYNOTES.</h5><p>In the past we\'ve had names like Michelle Obama, John Cena, Beth Comstock, Brené Brown, and Shonda Rhimes on the keynote stage. This year, more keynoters will inspire you with their visions for the future of marketing, sales, and business.</p><a>See 2018 Speakers</a>',
          image: ''
        },
        {
          content: '<h5>EDUCATIONAL BREAKOUT SESSIONS.</h5><p>INBOUND 2018 featured almost 300 breakout sessions from some of the biggest names and brightest minds in sales and marketing. INBOUND 2018 was packed with dozens of new tactics to take your business to the next level—and 2019 will be too.</p><a>See 2018 Agenda</a>',
          image: ''
        },
        {
          content: '<h5>FUN, FRIENDS, FOOD.</h5><p>There\'s more to INBOUND than just great content—it\'s also a lot of fun! How could it not be with amazing entertainment (like Tiffany Haddish in 2017 and 2 Dope Queens in 2018), happy hours and parties, and food truck lunches. INBOUND isn\'t just 24,000+ fellow attendees: it\'s 24,000+ of your new best friends.</p><a>Learn More</a>',
          image: ''
        }
      ]
    }
  }
}
</script>

<style lang="sass" scoped>
section.spilt-section
  background-color: #431a4f
  min-height: 150vh
  padding-bottom: 4rem
  position: relative
  background-image: url(//cdn2.hubspot.net/hubfs/146726/assets/images/backgrounds/bg-dotted.png)
  background-repeat: initial
  .container
    h2
      font-size: 2.7rem
      // line-height: 1.3rem
      text-align: center
      margin-top: 6rem

</style>
