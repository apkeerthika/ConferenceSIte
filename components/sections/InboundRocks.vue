<template lang="pug">
section.inbound-rocks
  .container
    .rocks-text
      h2 Inbound Rocks
      h3.dope-queens FEATURING 2 DOPE QUEENS
      h6.artists PHOEBE ROBINSON & JESSICA WILLIAMS
    .rocks-image
      img(src="https://www.inbound.com/hs-fs/hubfs/INBOUND18_2DopeQueens_Clipped_JP.png?t=1540589515044&width=471&name=INBOUND18_2DopeQueens_Clipped_JP.png")
</template>


<style lang="sass" scoped>
@import 'assets/styles/inbound'

section.inbound-rocks
  background-color: $inbound-darkblue
  color: $white
  background-image: url('//cdn2.hubspot.net/hubfs/146726/assets/images/backgrounds/bg-spray-v3.svg')
  background-repeat: no-repeat
  background-position: 5% 100%
  background-size: contain
  .container
    @include spread
    flex-direction: row-reverse
    padding: 0 !important
    .rocks-image
      flex: 1
      img
        width: 100%
        margin: 0 auto
    .rocks-text
      .dope-queens, .artists
        margin: 0.5em 0
      .dope-queens
        font-size: 1.25rem
        font-weight: 300
        margin: 1em 0 0.5em 0
      .artists
        font-weight: 400
        font-size: 0.8rem
      @media (min-width: 768px)
        text-align: left
        flex: 1
        padding-left: $space*8
</style>