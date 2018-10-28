<template lang="pug">
section.sponsors
  .container
    .cta-inner
      h3 INTERESTED IN BECOMING A SPONSOR?
      a.btn.btn-alt Learn More
</template>

<style lang="sass" scoped>
@import 'assets/styles/inbound'

section.sponsors
  background-color: $inbound-red
  color: $white

.cta-inner
  @include flex
  justify-content: center
  h3
    padding-right: 1.5em
  a
    padding: 1.49em 5.1em !important
</style>