<template lang="pug">
section.moments
  .container
    h2 Best of inbound 2018
    h4 SOME OF OUR FAVORITE MOMENTS
    ul.momento
      li.moment(v-for="(m, i) in moments", :key="i", :class="m.class")
        .thumb
          img(:src="m.image")
        .content
          p {{ m.keynote_name }}
          p {{ m.sub_name }}
</template>

<script>
export default {
  data () {
    return {
      moments: [
        {
          image: 'https://www.inbound.com/hs-fs/hubfs/Metoo%20Wide.jpg?t=1540589515044&width=710&name=Metoo%20Wide.jpg',
          keynote_name: 'Tarana Burke & Emily Chang Keynote',
          sub_name: 'Tarana Burke & Emily Chang',
          class: 'featured'
        },
        {
          image: 'https://www.inbound.com/hs-fs/hubfs/ScottHarrison-2.jpg?t=1540589515044&width=340&name=ScottHarrison-2.jpg',
          keynote_name: 'Scott Harrison Keynote',
          sub_name: 'Scott Harrison',
        },
        {
          image: 'https://www.inbound.com/hs-fs/hubfs/Image%20from%20iOS%20(7).jpg?t=1540589515044&width=340&name=Image%20from%20iOS%20(7).jpg',
          keynote_name: 'Chimamanda Ngozi Adichie Keynote',
          sub_name: 'Chimamanda Ngozi Adichie'
        },
        {
          image: 'https://www.inbound.com/hs-fs/hubfs/Image%20from%20iOS%20(6).jpg?t=1540589515044&width=338&name=Image%20from%20iOS%20(6).jpg',
          keynote_name: 'Mo Gawdat Spotlight',
          sub_name: 'Mo Gawdat'
        },
        {
          image: 'https://www.inbound.com/hs-fs/hubfs/AlexRod.jpg?t=1540589515044&width=338&name=AlexRod.jpg',
          keynote_name: 'Alex Rodriguez Spotlight',
          sub_name: 'Alex Rodriguez'
        }
      ]
    }
  }
}
</script>

<style lang="sass" scoped>
@import 'assets/styles/inbound'

.moments
  padding-top: $space*5
  padding-bottom: $space*5
  .container
    padding: 0 !important

.momento
  border: none !important
  @include reset
  @include spread
  flex-wrap: wrap


li.moment
  width: 350px
  margin-bottom: 15px
  &.featured
    width: 715px
  .thumb
    display: block
    height: 250px
    overflow: hidden
    text-align: center
    position: relative
    img
      @include absolute
      max-height: none
      max-width: none
      width: 110%
  .content
    background-color: $inbound-blue
    color: $white
    padding: 1.5em
    height: 120px
    text-align: left

</style>