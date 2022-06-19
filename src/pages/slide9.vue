<template lang="pug">
slide
  div.flex.flex-col
    h1 Immutable Objects

    slide2sides
      template(v-slot:left)
        example
          immutableobjects

      template(v-slot:right)
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
