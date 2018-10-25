<template lang="pug">
.page
  hero
  Content
  Speakers

</template>


<script>
import Speakers from '~/components/Speakers.vue'
import Hero from '~/components/Hero.vue'
import Content from '~/components/Content.vue'
export default {
  components: {
    Speakers,
    Hero,
    Content
  }
}
</script>

<style lang="sass" scoped>
@import 'assets/styles/inbound'

</style>
