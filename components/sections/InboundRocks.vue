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
  .container
    // @include spread
    padding-bottom: 0
    .rocks-image
      background-image: url('//cdn2.hubspot.net/hubfs/146726/assets/images/backgrounds/bg-spray-v3.svg')
      background-size: 100%
      background-repeat: no-repeat
      background-position: center center
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
</style>