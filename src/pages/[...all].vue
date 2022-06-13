<script setup lang="ts">

</script>

<template lang="pug">
main
  p hi
</template>

<style lang="sass">
:root
  --bg-explanation: #299D61
  --color-light: #9ACE99
  --accent: #0a2e1b

.custom-width
  width: 40%
  min-width: 300px

.steps-width
  width: 40%
  p
    @apply ml-4

@media screen and (max-width: 768px)
  .steps-width
    width: 100%

#video
  width: 100%
  aspect-ratio: 16 / 10

.extra
  @apply shadow-xl border-rounded p-5 m-2 bg-white

#explanation
  min-height: 100vh
  background: #c0e1e9
  h3
    color: var(--accent)
    margin-top: 0px

  h2
    //color: #0d3a23

.rainbow-box
  border: 5px solid transparent
  border-image: linear-gradient(to bottom right, #b827fc 0%, #2c90fc 25%, #b8fd33 50%, #fec837 75%, #fd1892 100%)
  border-image-slice: 1
  margin: 20px auto
</style>
