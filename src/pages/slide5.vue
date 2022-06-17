<template lang="pug">
slide.flex
  div.flex.flex-col
    h1 Objekt-polymorphismus und Subtyping
    .flex.h-100
      div(class="w-1/2")
        h2.heading Objektpolymorphismus
        ul.pl-5
          li Row Polymorphism
      div.divider
      div(class="w-1/2")
        h2.heading Subtyping
        ul.pl-5
          li Width Subtyping
          li Depth Subtyping
          li Polymorphic Variant Subtyping
</template>

<style lang="sass" scoped>
.heading
  @apply p-4 text-center

.divider
  @apply border-r-2 border-gray-300 mx-10
</style>
