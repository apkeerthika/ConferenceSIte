<template lang="pug">
section.app-header
  .container
    .logo
      nuxt-link(to="/")
        img(src="https://www.inbound.com/hubfs/assets/logos/INBOUND_2019_Logo_KO.svg?t=1540347310091", alt="Logo")
    nav.navigation
      .primary
        a About
        a Agenda
        a Attend
        a Watch
        a Help
      .secondary
        a(href="/register") Register
</template>

<script>
export default {
  
}
</script>

// <style lang="sass">
// @import 'assets/styles/inbound'

// .app-header + section
//   margin-top: $header-height
// </style>

<style lang="sass" scoped>
@import 'assets/styles/inbound'

section.app-header
  @include fixed-n
  height: $header-height
  margin-top: $space*1.5
  color: $white
  .container
    
    @include spread

section.app-header
  .logo
    width: 15rem
  .navigation
    @include flex
    .primary a, .secondary a
      margin: 0 $space
      font-weight: bold
      text-transform: uppercase
      curosr: pointer
    .secondary a
      border: 2px solid $white
      padding: $space*0.7 $space*2
      text-decoration: none
      &:hover
        background: rgba(255,255,255,0.2)
        color: $white
</style>
