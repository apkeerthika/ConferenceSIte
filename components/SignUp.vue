<template lang="pug">
section.sign-up
  .container
    h3.h3 SignUp For Inbound Updates
    .updates
      .input
        input(type="email", name="email" required, placeholder="you@yourDomain.com")
        span
          button.btn.btn-primary SignUp
    .rich-text
      p We're committed to your privacy. INBOUND uses the information you provide to us to contact you about upcoming and future INBOUND events. You may unsubscribe from these communications at any time. We do not use this information to market or sell you HubSpot products or services, and do not subscribe you to any HubSpot communications. For more information, check out our Privacy Policy.
</template>

<script>
export default {

}
</script>


<style lang="sass" scoped>
@import 'assets/styles/inbound'

section.sign-up
  // min-height: 45vh
  background-color: #501a50
  background-image: url('http://cdn2.hubspot.net/hubfs/146726/assets/images/backgrounds/bg-lens-flare.png')
  background-repeat: no-repeat
  background-size: cover
  background-position: bottom right
  padding: 4.1em 0
  .container
    text-transform: uppercase
    text-align: center
    .updates
      text-align: center
      margin-top: $space
      input
        width: 40% !important
        background-color: #ececf5
        color: #190a35
        font-weight: 600
        box-sizing: border-box
        transition: 0.5s ease border-color
        border-color: transparent
        box-shadow: none
        border-width: 3px
        padding: $space
        height: $space*3
        border-radius: 0
      span
        button
          height: 3rem
    .rich-text
      margin-top: $space*2
      p
        line-height: 1.5 !important
        font-size: 0.7rem
        letter-spacing: 0.01rem
        text-transform: none !important
        // text-align: center !important
</style>
