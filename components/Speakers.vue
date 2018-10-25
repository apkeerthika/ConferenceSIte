<template lang="pug">
.speakers-section
  h1 FEATURED 2018 SPEAKERS
  .main-speakers
    .card(v-for="speaker in mainSpeakers ") 
      img(:src="speaker.pic")
      .content
        h2 {{ speaker.name }}
        h3 {{ speaker.topic }}
</template>
<script>
export default {
  data() {
    return{
      mainSpeakers:[
         {name:'Billgates', topic:'Award Contents', pic: 'https://via.placeholder.com/300x300'},
         {name:'Billgates', topic:'Award Contents', pic: 'https://via.placeholder.com/300x300'},
         {name:'Billgates', topic:'Award Contents', pic: 'https://via.placeholder.com/300x300'},
         {name:'Billgates', topic:'Award Contents', pic: 'https://via.placeholder.com/300x300'},
         {name:'Billgates', topic:'Award Contents', pic: 'https://via.placeholder.com/300x300'},
         {name:'Billgates', topic:'Award Contents', pic: 'https://via.placeholder.com/300x300'}
      ]
    }
  }
}
</script>
<style lang="sass" scoped>
.speakers-section
  .main-speakers
        

</style>
