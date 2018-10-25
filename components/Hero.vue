<template lang="pug">
section.hero
  .container
    .banner-text
      h1 See You Next Year
      h6 SEPTEMBER 3-6, 2019 | BOSTON, MA
      .cta
        a Watch 2017 RECAP
        a Registerr for 2019
  AppHeader
</template>

<script>
import AppHeader from '~/components/common/AppHeader'

export default {
  components: {
    AppHeader
  }
}
</script>

<style lang="sass" scoped>
@import 'assets/styles/inbound'
section.hero
  padding-top: $space*15
  height: auto
  min-height: 100vh
  background-image: url('https://www.inbound.com/hubfs/INBOUND_DAY2_117%20copy.jpg?t=1540347310091')
  background-repeat: no-repeat
  background-size: cover
  color: $white
  .container
    z-index: 2
    text-transform: uppercase
    .banner-text
      max-width: 60rem
      margin: 0 auto
      text-align: center
      > h1
        color: $white
        font-size: 3.5rem
        font-weight: 600
        letter-spacing: 1.5rem
        line-height: 5rem
      > h6
        font-weight: bold
        letter-spacing: 0.2rem
        line-height: 2rem
        font-size: 1.5rem
      .cta
        margin-bottom: $space*4

</style>
