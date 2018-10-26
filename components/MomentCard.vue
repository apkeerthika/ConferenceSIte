<template lang="pug">
li.moment(:class="{featured: isFeatured }")
  a.thumb
    img(:src="content.img")
  .content
    h4 
      a {{ content.name }}
    h6 {{ content.subname }}
</template>

<script>
export default {
  props: ['content', 'isFeatured']
}
</script>

<style lang="sass" scoped>
@import 'assets/styles/inbound.sass'

li.moment
  width: 350px
  margin-bottom: 15px
  &.featured
    width: 715px
  .thumb
    display: block
    height: 250px
    background: #CCC
    overflow: hidden
    text-align: center
    position: relative
    img
      @include absolute
      max-height: none
      max-width: none
      width: 110%
  .content
    background: $accent-color3
    letter-spacing: 1px
    line-height: 1.125
    color: $white
    font-weight: 600
    padding: 1.9em 3.18em 1.9em 1.9em
    height: 120px
    h4
      text-transform: uppercase
      font-size: 1rem
      font-weight: 700
      line-height: 1.25rem
    h6
      font-weight: 300
</style>

