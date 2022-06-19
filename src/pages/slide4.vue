<template lang="pug">
slide
  div.flex.flex-col
    h1 Objekte in OCaml
    .flex.h-100
      div(class="w-1/2")
        example
          objectexample
      ul(class="w-1/2")
        //li Objekte und Klassen sind eine Möglichkeit von OCaml OOP anzuwenden
        li Objekte haben nicht wie andere Sprachen Klassentypen, sondern werden durch ihren
          span  Objekttyp
          |  beschrieben
        li
          | Der
          span  Objekttype
          |  wird durch die bereitgestellten Methoden festgelegt
        li
          span Methoden
          |  werden mit dem #-Operator aufgerufen
</template>

<!--

- Objekte haben eine bestimmte Syntax mit der man sowohl Attribute wie auch Methoden definieren kann
- Als Konstruktor muss man selber eine Funktion erstellen, die das erzeugte Objekt zurückgibt
- Der Objekttyp wird durch die bereitgestellten Methoden festgelegt
	- "classes are not types"
	- we use "object types"
		- enclosed in `< ... >`
		- The `..`(row variable) in the inferred object types are ellipses, standing for other unspecified methods that the object may have.
		- Objekttypen können mit Typannotation geschlossen werden (let area_closed (sq: < width : int >) = sq#width * sq#width;;)
- Invoke a method with `#`
	- zero parameters allowed
 -->
