<template lang="pug">
section.hero
  .container
    .banner-text
      h1 See You Next Year
      h6 SEPTEMBER 3-6, 2019 | BOSTON, MA
      .cta
        a.recap Watch 2017 RECAP
        a.register Registerr for 2019
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
        margin-top: $space*6
        font-weight: bold
        > a
          border: 1px solid $white
          padding: $space*2  $space*5
          border-width: 0.2rem
          display: inline-block
          cursor: pointer
          &:hover
            background-color: rgba(255,255,255,0.2)
            color: $white
        .register
          background: linear-gradient(to right, #ba2027, #a71072, #ea088b, #eb2155, #ba2027) 160% 0 repeat-x,linear-gradient(to top, #ba2027, #a71072, #ea088b, #eb2155, #ba2027) 100% 20% repeat-y,linear-gradient(to left, #ba2027, #a71072, #ea088b, #eb2155, #ba2027) 10% 100% repeat-x,linear-gradient(to bottom, #ba2027, #a71072, #ea088b, #eb2155, #ba2027) 0% 10% repeat-y
          background-size: 300% .1875em,.1875em 300%
          animation: rotateGradient 20s infinite linear
          border: 0
          padding: $space*2  $space*5
          display: inline-block
          margin-left: $space*5
        .recap
          &:after
            content: '\25B6'
            display: inline-block
            position: relative
            top: 0
            left: 1.31em
            width: 0.45em
</style>
