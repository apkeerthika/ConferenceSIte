<template lang="pug">
section.speakers-section
  .container
    h1 FEATURED 2018 SPEAKERS
    .main-speakers
      .card(v-for="speaker in mainSpeakers ") 
        img(:src="speaker.pic")
        .content
          h3 {{ speaker.name }}
          p {{ speaker.topic }}
    .sub-speakers
      .card(v-for="speaker in subSpeakers ") 
        img(:src="speaker.pic")
        .content
          h3 {{ speaker.name }}
          p {{ speaker.topic }}      
</template>
<script>
export default {
  data() {
    return{
      mainSpeakers:[
         {name:'CHIMAMANDA NGOZI ADICHIE', topic:'Award-Winning Novelist & Writer', pic: 'https://www.inbound.com/hs-fs/hubfs/Keynote%20Profile%201.png?t=1540417776371&width=338&name=Keynote%20Profile%201.png'},
         {name:'DEEPAK CHOPRA', topic:'Best-Selling Author and Founder, Chopra Foundation', pic: 'https://www.inbound.com/hs-fs/hubfs/Keynote%20Profile%202-1.png?t=1540417776371&width=676&name=Keynote%20Profile%202-1.png'},
         {name:'BETH COMSTOCK', topic:'Former Vice Chair, GE', pic: 'https://www.inbound.com/hs-fs/hubfs/Keynote%20Profile%205.png?t=1540417776371&width=676&name=Keynote%20Profile%205.png'},
         {name:'SCOTT HARRISON', topic:'Founder & CEO, charity:water', pic: 'https://www.inbound.com/hs-fs/hubfs/Keynote%20Profile%204.png?t=1540417776371&width=507&name=Keynote%20Profile%204.png'},
         {name:'BRIAN HALLIGAN & DHARMESH SHAH', topic:'Co-Founders, HubSpot', pic: 'https://www.inbound.com/hs-fs/hubfs/assets/images/speakers/Brian-Halligan-Dharmesh-Shah-INBOUND.png?t=1540417776371&width=507&name=Brian-Halligan-Dharmesh-Shah-INBOUND.png'},
         {name:'SHONDA RHIMES', topic:'Award Winning Writer, Executive Producer, and Best Selling AuthorT', pic: 'https://www.inbound.com/hs-fs/hubfs/INBOUND18_ShondaRhimes_KeynoteProfile-1.png?t=1540417776371&width=507&name=INBOUND18_ShondaRhimes_KeynoteProfile-1.png'}
      ],
      subSpeakers:[
        {name:'TARANA BURKE', topic:'Founder of the \'me too.\' Movement', pic:'https://www.inbound.com/hs-fs/hubfs/Spotlight%20Profile%2033-1.png?t=1540417776371&width=563&name=Spotlight%20Profile%2033-1.png'},
        {name:'EMILY CHANG', topic:'Author, Brotopia & Executive Producer, Bloomberg Technology', pic:'https://www.inbound.com/hs-fs/hubfs/EmilyChang-INBOUND-color.jpg?t=1540417776371&width=450&name=EmilyChang-INBOUND-color.jpg'},
        {name:'TROY CARTER', topic:'Founder & CEO, Atom Factory', pic:'https://www.inbound.com/hs-fs/hubfs/TroyCarter-INBOUND-color.jpg?t=1540417776371&width=450&name=TroyCarter-INBOUND-color.jpg'},
        {name:'MO GAWDAT', topic:'Chief Business Officer, Google X', pic:'https://www.inbound.com/hs-fs/hubfs/Mo_Gawdat_Google.png?t=1540417776371&width=450&name=Mo_Gawdat_Google.png'},
        {name:'ESTHER PEREL', topic:'Psychotherapist and Host, Where Should We Begin?', pic:'https://www.inbound.com/hs-fs/hubfs/INBOUND18_EstherPerel_SpotlightProfile-1.png?t=1540417776371&width=563&name=INBOUND18_EstherPerel_SpotlightProfile-1.png'},
        {name:'JULIE RICE', topic:'Co-Founder, Soulcycle & Chief Brand Officer, WeWork', pic:'https://www.inbound.com/hs-fs/hubfs/Spotlight%20Profile%2023-3.png?t=1540417776371&width=450&name=Spotlight%20Profile%2023-3.png'},
        {name:'ALEX RODRIGUEZ', topic:'Founder & Chief Executive Officer, A-Rod Corp', pic:'https://www.inbound.com/hs-fs/hubfs/Spotlight.png?t=1540417776371&width=563&name=Spotlight.png'},
        {name:'LENA WAITHE', topic:'Emmy Award Winning Writer, Producer, and Actress', pic:'https://www.inbound.com/hs-fs/hubfs/Lena%20Waithe.png?t=1540417776371&width=338&name=Lena%20Waithe.png'}
      ]
    }
  }
}
</script>
<style lang="sass" scoped>
@import 'assets/styles/inbound'
section.speakers-section
  h1
    text-align: center
  .container
    .main-speakers
      display: flex
      flex-wrap: wrap
      justify-content: center
      margin-left: auto
      margin-right: auto
      width: 100%
      .card
        width: 33.33333333%
        padding: 1rem
        @media(max-width: $breakpoint-tab-1)
          width: 50%
        img
          width: 100%
          display: block
        .content
          background-color: $brand-color
          height: $space*10
          padding: $space*2
          color: $white
          line-height: 2rem
          > h3
            color: $white
    .sub-speakers
      display: flex
      flex-wrap: wrap
      justify-content: center
      margin-left: auto
      margin-right: auto
      width: 100%
      margin-top: $space*2
      .card
        width: 24.9%
        padding: $space
        img
          width: 100%
          display: block
        .content
          background-color: $brand-color
          height: $space*10
          padding: $space*2
          color: $white
          line-height: 2rem
          h3, p
            color: $white
            // margin-left: 1rem      
          
         
      

</style>
