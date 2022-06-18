<template lang="pug">
slide.flex
  div.flex.flex-col
    h1 Row Poly vs. Subtyping

    slide2sides
      template(v-slot:left)
        h2 Row Poly

      template(v-slot:right)
        h2 Subtyping
        ul
          li
            | Die Syntax mit
            |
            code {...}
            |  ist nur in Methoden von Objekten erlaubt und erzeugt ein neues Objekt
          li
            span Methodenimplementationen
            |
            | können nicht durch die Syntax von
            |
            code {...}
            |  verändert werden
</template>
