<template lang="pug">
.page
  section.app-header
    .container
      h1 Header
  section.app-main
    .container
      section.content
        h1 Main
        h2 Main
        h3 Main
        h4 Main
        h5 Main
        h6 Main
        a link
      section.content
        button.btn READ ME
      section.dark.content
        button.btn.btn-alt READ ME
      section.content
        button.btn.btn-primary READ ME
      section.content
        button.btn.btn-big READ ME
      p Colors that are opposite each other on the color wheel are considered to be complementary colors (example: red and green). The high contrast of complementary colors creates a vibrant look especially when used at full saturation. This color scheme must be managed well so it is not jarring. Complementary colors are tricky to use in large doses, but work well when you want something to stand out. Complementary colors are really bad for text.


  section.app-footer
    .container
      h1 Footer
</template>

<style lang="sass" scoped>
@import 'assets/styles/config/colors'
@import 'assets/styles/config/layout'
// @import 'assets/styles/config/shadows'
// @import 'assets/styles/config/typography'
// @import 'assets/styles/config/z'
// @import 'assets/styles/config/breakpoints'

// @import 'mixin/fixed'
// @import 'mixin/absolute'
// @import 'mixin/flex'
// @import 'mixin/reset'
// @import 'mixin/theme'
// @import 'mixin/underline'
// @import 'mixin/animated'

// @import 'base/base'
// @import 'base/form'
// @import 'base/form-input'
// @import 'base/typography'
@import 'assets/styles/base/buttons'

// @import 'components/modal'

$page-width: 1080px
$space: 1rem

.dark
  background: $inbound-violet

section.content
  padding: 1rem

.container
  max-width: $page-width
  margin: auto
  @media (max-width: $page-width)
    padding: 0 $space

.app-header
  background: $brand-color
  color: $white
  h1
    margin-top: 0

.app-footer
  background: $brand-color
  color: $white
</style>

<style lang="sass">
body
  margin: 0
  padding: 0
</style>


