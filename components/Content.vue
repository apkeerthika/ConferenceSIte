<template lang="pug">
section.best-of-2018
  .container
    .heading
      h1 BEST OF IMBOUND 2018
      h3 SOME OF OUR FAVORITE MOMENTS
    
    ul.moments
      li
        a
          img(:src="featured.img")
        .content
          h4 
            a {{ featured.name }}
          h6 {{ featured.subname }}
      li(v-for="content in contents")
        a
          img(:src="content.img")
        .content
          h4 
            a {{ content.name }}
          h6 {{ content.subname }}
    .button
      a SEE MORE CONTENT

</template>
<script>
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

          
.moments
  @include flex 
  flex-wrap: wrap
  padding: 2.87em 0
  @include reset

  li
    // width: 340px
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

.best-of-2018
  .button
    border: 1px solid #190a35
    border-width: .1875em
    padding: 1.49em 5.1em
    width: 31%
    justify-content: center
    &:hover
      background-color: #190a35
      color: #fff


</style>
