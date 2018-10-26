<template lang="pug">
.page
  hero
  SignUp
  Content
  Speakers
  SpiltSection
</template>


<script>
import Hero from '~/components/Hero'
import SignUp from '~/components/SignUp'
import Content from '~/components/Content'
import Speakers from '~/components/Speakers'
import SpiltSection from '~/components/SpiltSection'
export default {
  components: {
    Hero,
    SignUp,
    Content,
    Speakers,
    SpiltSection
  }
}
</script>

<style lang="sass">
@import 'assets/styles/inbound'
body
  margin: 0 !important
</style>
