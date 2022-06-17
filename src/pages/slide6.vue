<template lang="pug">
slide.flex
  div.flex.flex-col
    h1 Row Polymorphism

    slide2sides
      template(v-slot:left)
        example
          objpolyexample

      template(v-slot:right)
        ul
          li Methoden können ohne explizite Typannotation angegeben werden da der Typ inferiert wird
          li
            code ..
            |  ist eine
            span  Row Variable
          li
            code &lt; pop : int option; .. >
            |  kann jedes Objekt sein, dass einen Methode
            |
            code pop
            |  mit der gezeigten Architektur hat
    slide2sides
      template(v-slot:left)
        example
          closedtypeex

      template(v-slot:right)
        ul
          li Objekttypen können explizit geschlossen werden
</template>
