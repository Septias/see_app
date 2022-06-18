<template lang="pug">
slide.flex
  div.flex.flex-col
    h1 Subtyping > Variance
    h2 Variance
    slide2sides
      template(v-slot:left)
        example
          variance
      template(v-slot:right)
        ul
          li Typen die aus Objekttypen kontruiert wurden können auch genötigt werden
          li We say that 'a list is covariant (in 'a), while 'a array is invariant.
    slide2sides
      template(v-slot:left)
        example
          variance2

    h2 Variance Annotations
    p TODO
</template>
