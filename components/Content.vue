<template lang="pug">
.pages
  h1 BEST OF IMBOUND 2018
    h5 SOME OF OUR FAVORITE MOMENTS
  .container
    ul(v-for="content in contents")
      li.list
        a()
          img(:src="content.img")
        .content
          h3 {{ content.name }}
          h6 {{ content.subname }}
          
      

</template>
<script>
export default {
  data() {
    return {
      contents:[
        {img: 'https://www.inbound.com/hs-fs/hubfs/Metoo%20Wide.jpg?t=1540247590317&width=710&name=Metoo%20Wide.jpg' , name:' Tarana Burke & Emily Chang Keynote' , subname:'Tarana Burke & Emily Chang'},
        {img: 'https://www.inbound.com/hs-fs/hubfs/ScottHarrison-2.jpg?t=1540247590317&width=170&name=ScottHarrison-2.jpg 170w, https://www.inbound.com/hs-fs/hubfs/ScottHarrison-2.jpg?t=1540247590317&width=340&name=ScottHarrison-2.jpg 340w, https://www.inbound.com/hs-fs/hubfs/ScottHarrison-2.jpg?t=1540247590317&width=510&name=ScottHarrison-2.jpg 510w, https://www.inbound.com/hs-fs/hubfs/ScottHarrison-2.jpg?t=1540247590317&width=680&name=ScottHarrison-2.jpg 680w, https://www.inbound.com/hs-fs/hubfs/ScottHarrison-2.jpg?t=1540247590317&width=850&name=ScottHarrison-2.jpg 850w, https://www.inbound.com/hs-fs/hubfs/ScottHarrison-2.jpg?t=1540247590317&width=1020&name=ScottHarrison-2.jpg 1020w' , name:'Scott Harrison Keynote' , subname:'Scott Harrison'},
        {img: 'https://www.inbound.com/hs-fs/hubfs/Image%20from%20iOS%20(7).jpg?t=1540247590317&width=170&name=Image%20from%20iOS%20(7).jpg 170w, https://www.inbound.com/hs-fs/hubfs/Image%20from%20iOS%20(7).jpg?t=1540247590317&width=340&name=Image%20from%20iOS%20(7).jpg 340w, https://www.inbound.com/hs-fs/hubfs/Image%20from%20iOS%20(7).jpg?t=1540247590317&width=510&name=Image%20from%20iOS%20(7).jpg 510w, https://www.inbound.com/hs-fs/hubfs/Image%20from%20iOS%20(7).jpg?t=1540247590317&width=680&name=Image%20from%20iOS%20(7).jpg 680w, https://www.inbound.com/hs-fs/hubfs/Image%20from%20iOS%20(7).jpg?t=1540247590317&width=850&name=Image%20from%20iOS%20(7).jpg 850w, https://www.inbound.com/hs-fs/hubfs/Image%20from%20iOS%20(7).jpg?t=1540247590317&width=1020&name=Image%20from%20iOS%20(7).jpg 1020w' , name:'Chimamanda Ngozi Adichie Keynote' , subname:'Chimamanda Ngozi Adichie'},
        {img: 'https://www.inbound.com/hs-fs/hubfs/Image%20from%20iOS%20(6).jpg?t=1540247590317&width=169&name=Image%20from%20iOS%20(6).jpg 169w, https://www.inbound.com/hs-fs/hubfs/Image%20from%20iOS%20(6).jpg?t=1540247590317&width=338&name=Image%20from%20iOS%20(6).jpg 338w, https://www.inbound.com/hs-fs/hubfs/Image%20from%20iOS%20(6).jpg?t=1540247590317&width=507&name=Image%20from%20iOS%20(6).jpg 507w, https://www.inbound.com/hs-fs/hubfs/Image%20from%20iOS%20(6).jpg?t=1540247590317&width=676&name=Image%20from%20iOS%20(6).jpg 676w, https://www.inbound.com/hs-fs/hubfs/Image%20from%20iOS%20(6).jpg?t=1540247590317&width=845&name=Image%20from%20iOS%20(6).jpg 845w, https://www.inbound.com/hs-fs/hubfs/Image%20from%20iOS%20(6).jpg?t=1540247590317&width=1014&name=Image%20from%20iOS%20(6).jpg 1014w' , name:'Mo Gawdat Spotlight' , subname:'Mo Gawdat'},
        {img: 'https://www.inbound.com/hs-fs/hubfs/AlexRod.jpg?t=1540247590317&width=169&name=AlexRod.jpg 169w, https://www.inbound.com/hs-fs/hubfs/AlexRod.jpg?t=1540247590317&width=338&name=AlexRod.jpg 338w, https://www.inbound.com/hs-fs/hubfs/AlexRod.jpg?t=1540247590317&width=507&name=AlexRod.jpg 507w, https://www.inbound.com/hs-fs/hubfs/AlexRod.jpg?t=1540247590317&width=676&name=AlexRod.jpg 676w, https://www.inbound.com/hs-fs/hubfs/AlexRod.jpg?t=1540247590317&width=845&name=AlexRod.jpg 845w, https://www.inbound.com/hs-fs/hubfs/AlexRod.jpg?t=1540247590317&width=1014&name=AlexRod.jpg 1014w' , name:'Alex Rodriguez Spotlight' , subname:'Alex Rodriguez'}
        
      ]
    }
  }

  
}
</script>
<style lang="sass" scoped>

@import 'assets/styles/inbound.sass'

.pages
  .container
    ul
      @include reset
      @include flex

      li
        background: $accent-color3
        color: $white

        a
        .content
          letter-spacing: 1px
          line-height: 1.125
          >h3
            color: $white
  


</style>
