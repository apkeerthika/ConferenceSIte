<template lang="pug">
section.best-of-2018
  .container
    .heading
      h1 BEST OF IMBOUND 2018
      h3 SOME OF OUR FAVORITE MOMENTS
    
    ul.moments
      moment-card(:content="featured", :isFeatured="true")
      moment-card(v-for="c in contents", :content="c")

    .button
      a SEE MORE CONTENT

</template>
<script>
import MomentCard from '@/components/MomentCard'
export default {
  data() {
    return {
      featured: {
        img: 'https://www.inbound.com/hs-fs/hubfs/Metoo%20Wide.jpg' , name:' Tarana Burke & Emily Chang Keynote' , subname:'Tarana Burke & Emily Chang'
      },
      contents:[
        {img: 'https://www.inbound.com/hs-fs/hubfs/ScottHarrison-2.jpg' , name:'Scott Harrison Keynote' , subname:'Scott Harrison'},
        {img: 'https://www.inbound.com/hs-fs/hubfs/Image%20from%20iOS%20(7).jpg' , name:'Chimamanda Ngozi Adichie Keynote' , subname:'Chimamanda Ngozi Adichie'},
        {img: 'https://www.inbound.com/hs-fs/hubfs/Image%20from%20iOS%20(6).jpg' , name:'Mo Gawdat Spotlight' , subname:'Mo Gawdat'},
        {img: 'https://www.inbound.com/hs-fs/hubfs/AlexRod.jpg' , name:'Alex Rodriguez Spotlight' , subname:'Alex Rodriguez'}
        
      ]
    }
  },
  components: {
    MomentCard
  }
}
</script>
<style lang="sass" scoped>

@import 'assets/styles/inbound.sass'

.best-of-2018
  padding: 2.87em 0
  .heading
    line-height: 1.1333
    letter-spacing: 0
    text-align: center
    h1
      color: black
      font-size: 45px
    h3
      font-size: 1.5rem
      margin-top: 0.55em

.best-of-2018
  .container
    padding: 0 !important
          
.moments
  border: none !important
  @include reset
  @include spread
  flex-wrap: wrap

.best-of-2018
  .button
    border: 1px solid #190a35
    border-width: .1875em
    padding: 1.49em 5.1em
    width: 350px
    margin: 2rem auto
    color: black
    text-align: center
    box-sizing: border-box
    &:hover
      background-color: #190a35
      color: #fff


</style>
