<template lang="pug">
.page
  hero
  SignUp
  Content
  Speakers
</template>


<script>
import Hero from '~/components/Hero'
import SignUp from '~/components/SignUp'
import Content from '~/components/Content'
import Speakers from '~/components/Speakers'
export default {
  components: {
    Hero,
    SignUp,
    Content,
    Speakers,
  }
}
</script>

<style lang="sass">
@import 'assets/styles/inbound'
body
  margin: 0 !important
</style>
