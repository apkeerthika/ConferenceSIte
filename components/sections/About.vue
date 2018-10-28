<template lang="pug">
section.about
  .container
    h2 What to expect from inbound
    ul
      li.section(v-for="(section, i) in about", :key="i")
        .image
          img(:src="section.image")
        .text
          h4 {{ section.title }}
          p {{ section.content }}
          a.button.btn-inbound {{ section.cta.label }}
</template>


<script>
export default {
  data () {
    return {
      about: [
        {
          image: 'https://www.inbound.com/hubfs/assets/images/backgrounds/INBOUND-piera-bow.png?t=1540589515044',
          title: 'INSPIRING KEYNOTES.',
          content: 'In the past we\'ve had names like Michelle Obama, John Cena, Beth Comstock, Brené Brown, and Shonda Rhimes on the keynote stage. This year, more keynoters will inspire you with their visions for the future of marketing, sales, and business.',
          class: 'speakers',
          cta: {
            label: 'See 2018 Speakers',
            url: ''
          }
        },
        {
          image: 'https://www.inbound.com/hubfs/assets/images/speakers/INBOUND-breakout-sessions.png?t=1540589515044',
          title: 'EDUCATIONAL BREAKOUT SESSIONS.',
          content: 'INBOUND 2018 featured almost 300 breakout sessions from some of the biggest names and brightest minds in sales and marketing. INBOUND 2018 was packed with dozens of new tactics to take your business to the next level—and 2019 will be too.',
          class: 'agenda',
          cta: {
            label: 'See 2018 Agenda',
            url: ''
          }
        },
        {
          image: 'https://www.inbound.com/hubfs/Ducks%20Text.jpg?t=1540589515044',
          title: 'FUN, FRIENDS, FOOD.',
          content: 'There\'s more to INBOUND than just great content—it\'s also a lot of fun! How could it not be with amazing entertainment (like Tiffany Haddish in 2017 and 2 Dope Queens in 2018), happy hours and parties, and food truck lunches. INBOUND isn\'t just 24,000+ fellow attendees: it\'s 24,000+ of your new best friends.',
          class: 'more',
          cta: {
            label: 'Learn More',
            url: ''
          }
        }
      ]
    }
  }
}
</script>


<style lang="sass" scoped>
@import 'assets/styles/inbound'

section.about
  background-color: $inbound-darkpurple
  background-image: url('//cdn2.hubspot.net/hubfs/146726/assets/images/backgrounds/bg-dotted.png')
  color: $white


.container
  .section
    .image
      height: 20rem
      width: 48%
    .text
      width: 49%
      text-align: left
      padding-left: $space*2
      margin-bottom: $space*2
      // a
      //   &:hover
      //     background: rgba(255,255,255,0.2)
      //     color: $white
      //     transition: 0.3s
      p
        margin-top: $space*1.5
        margin-bottom: $space*3.5

.container
  @media (min-width: 768px)
    .section
      @include flex
      padding: $space
      &:nth-child(odd)
        flex-direction: row-reverse
        .text
          flex: 1
          padding-right: $space
</style>
