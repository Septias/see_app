<script lang="ts" setup>
const points = [
  {
    title: 'Abstraction',
    content: 'The details of the implementation are hidden in the object, and the external interface is just the set of publicly accessible methods',
  },
  {
    title: 'Dynamic lookup',
    content: 'When a message is sent to an object, the method to be executed is determined by the implementation of the object, not by some static property of the program. In other words, different objects may react to the same message in different ways.',
  },
  {
    title: 'Subtyping',
    content: 'If an object `a` has all the functionality of an object `b`, then we may use `a` in any context where `b` is expected.',
  },
  {
    title: 'Inheritance',
    content: 'The definition of one kind of object can be reused to produce a new kind of object. This new definition can override some behavior, but also share code with its parent.',
  },
  {
    title: 'Open recursion',
    content: 'An object’s methods can invoke another method in the same object using a special variable (often called `self` or `this`). When objects are created from classes, these calls use dynamic lookup, allowing a method defined in one class to invoke methods defined in another class that inherits from the first.',
  },
]
</script>

<template lang="pug">
slide
  h1.mb-10 Fundamentals of OOP
  .grid.grid-cols-3.gap-4
    .rounded-xl.p-5(v-for="point in points")
      h2.text-xl {{point.title}}
      p.text-sm {{point.content}}
</template>

