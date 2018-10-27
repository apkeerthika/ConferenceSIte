<template lang="pug">
.page.home
  AppHeader
  Hero
  SignUp
  Moments
  About
  Speakers
  InboundRocks
  Agenda
  Sponsors
  AppFooter
</template>


<script>
import AppHeader from '~/components/sections/AppHeader'
import Hero from '~/components/sections/Hero'
import SignUp from '~/components/sections/SignUp'
import Moments from '~/components/sections/Moments'
import About from '~/components/sections/About'
import Speakers from '~/components/sections/Speakers'
import InboundRocks from '~/components/sections/InboundRocks'
import Agenda from '~/components/sections/Agenda'
import Sponsors from '~/components/sections/Sponsors'
import AppFooter from '~/components/sections/AppFooter'
export default {
  components: {
    AppHeader,
    Hero,
    SignUp,
    Moments,
    About,
    Speakers,
    InboundRocks,
    Agenda,
    Sponsors,
    AppFooter
  }
}
</script>

<style lang="sass" scoped>
@import 'assets/styles/inbound'

</style>


<style lang="sass">
body
  margin: 0
  padding: 0
</style>


