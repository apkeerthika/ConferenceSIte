<template lang="pug">
section.agenda
  .container
    h2 2018 Agenda
    .content
      ul
        li
          span(@click="select(i)", v-for="(day, i) in data", :key="i") {{ day.day }} 
            .date {{ day.date }}
      .sessions(v-if="selected === i", v-for="(day, i) in data", :key="i")
        .session(v-for="(s, i) in day.sessions", :key="i")
          p.time
            span {{ s.start_time }} 
            span(v-if="s.end_time") — {{ s.end_time }}
          .marker(:class="s.class")
            img.image(v-if="s.bg", :src="s.bg")
          p.text {{ s.title }}
    .cta
      a.btn.btn-alt See The full 2018 agenda
</template>

<script>
import session from '~/components/sections/session.js'
export default {
  data () {
    return {
      data: session,
      selected: 0
    }
  },
  methods: {
    select (i) {
      this.selected = i
    }
  }
}
</script>


<style lang="sass" scoped>
@import 'assets/styles/inbound'

section.agenda
  background-color: $inbound-blue
  color: $white
  padding: $space*5
  .content
    padding-top: $space*5


.sessions
  padding-top: $space*3
  .session
    @include spread
    .time, .text
      flex: 1
    .time
      text-align: right
      padding-right: $space*3
    .text
      text-align: left
      padding-left: $space*3
      font-size: 1rem

.cta
  padding-top: $space*7
  a
    padding: $space*1.75 $space*5 !important

.marker
  background: transparent
  width: 1.2rem
  height: 1.2rem
  border-radius: 50%
  border: 4px solid $white
  margin: $space*2
  position: relative
  &:after
    content: ""
    display: block
    width: 4px
    height: 4.5rem
    background: $white
    @include absolute-n
    top: 100%

.session
  &:last-child
    .marker
      &:after
        display: none

.marker
  &.image
    background-size: contain
    width: 3.5rem
    height: 3.5rem
    margin: $space !important

.marker
  &.skyblue
    background: $inbound-lightblue
    width: 1.2rem
    height: 1.2rem
    border-radius: 50%
    border: 4px solid $white


.marker
  &.red
    background: $inbound-red
    width: 1.2rem
    height: 1.2rem
    border-radius: 50%
    border: 4px solid $white

//Desktop
ul
  display: flex
  li
    span
      letter-spacing: 2px
      font-weight: 600
      font-size: 1.5rem
      cursor: pointer
    @media (min-width: 768px)
      @include flex
      span
        display: inline-flex
        justify-content: space-around
        cursor: pointer
        padding: $space*2
</style>