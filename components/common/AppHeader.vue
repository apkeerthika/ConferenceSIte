<template lang="pug">
section.app-header(:class="{dark: isScroll}")
  .container
    .logo
      nuxt-link(to="/")
        img(src="https://www.inbound.com/hubfs/assets/logos/INBOUND_2019_Logo_KO.svg?t=1540347310091", alt="Logo")
    nav.navigation
      .primary
        a About
        a Attend
        a Agenda
        a Watch
        a Help
      .secondary
        a(href="/register") Register
</template>

<script>
export default {
  data () {
    return {
      isScroll: false
    }
  },
  created () {
    if (process.client)
      window.addEventListener('scroll', this.handleScroll);
  },
  destroyed () {
    window.removeEventListener('scroll', this.handleScroll);
  },
  methods: {
    handleScroll () {
      this.isScroll = window.scrollY >= 60
    }
  }
}
</script>

<style lang="sass" scoped>
@import 'assets/styles/inbound'

section.app-header
  @include fixed-n
  height: $header-height - 1
  color: $white
  .container
    @include spread
    padding-top: $space*1.3
section.app-header
  .logo
    width: 15rem
  .navigation
    @include flex
    .primary a, .secondary a
      // margin: 0 $space
      text-transform: uppercase
    .secondary a
      border: 2px solid $white
      padding: $space*0.5 $space*1.5
      text-decoration: none
      display: inline-block
      &:hover
        background: rgba(255,255,255,0.2)
        color: $white


.app-header.dark
  background: $brand-color
  transition: background-color 0.35s, border 0.35s
  position: fixed
  top: 0
  left: 0
  width: 100%
  z-index: 20

.navigation a
  &:hover
    border-bottom: 2px solid $white
</style>
