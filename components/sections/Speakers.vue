<template lang="pug">
section.speakers
  .container
    h2 Featured 2018 Speakers
    .profile-item(v-for="(s, i) in data", :key="i")
      .featured-profile(v-for="(f, j) in s.featured_speakers", :key="j")
        .image
          img(:src="f.image")
        .caption
          p {{ f.name }}
          p {{ f.company }}
      .profile-sub(v-for="(s, k) in s.speakers", :key="k")
        .image
          img(:src="s.image")
        .caption
          p {{ s.name }}
          p {{ s.company }}
</template>


<script>
import speaker from './speaker'

export default {
  data () {
    return {
      data: speaker
    }
  }
}
</script>

<style lang="sass" scoped>
@import 'assets/styles/inbound'

.profile-item
  display: flex
  justify-content: flex-start
  flex-wrap: wrap

.featured-profile
  width: 31.33%
  display: flex
  flex-flow: column
  position: relative
  .caption
    background-color: $inbound-violet
    color: $white
    padding: 1.6em 1.2em
    display: inline-block
    position: relative
    width: 100%
    overflow: hidden
    flex: 1 1 auto
    text-align: left
    @media (max-width: 768px)
      p
        font-size: 2vw

.featured-profile
  margin-left: 3.00005%
  &:first-child
    margin-left: 0
  &:nth-child(3n+1)
    margin-left: 0
  @media (max-width: 768px)
    &:nth-child(odd)
      margin-left: 0
    &:nth-child(even)
      margin-left: 3%


.featured-profile
  @media (max-width: 768px)
    width: 48%

.profile-sub
  &:nth-child(4n+2)
    margin-left: 2.8%
  &:nth-child(4n+4)
    margin-left: 2.8%
  &:nth-child(4n+5)
    margin-left: 2.8%
.profile-sub
  margin-top: $space*3
  width: 22.9%
  display: flex
  flex-flow: column
  position: relative
  @media(max-width: 768px)
    width: 100%
  .image
    img
      width: 100%
      @media(max-width: 768px)
        height: 100%
  .caption
    background: $inbound-violet
    color: $white
    display: inline-block
    position: relative
    width: 100%
    overflow: hidden
    flex: 1 1 auto
    box-sizing: border-box
    padding: 1.6em
    text-align: left


.profile-sub
  @media (max-width: 768px)
    flex-flow: row
    // .caption
    //   display: block
</style>