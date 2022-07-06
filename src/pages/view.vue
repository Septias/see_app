<script lang="ts" setup>
const fahrten = [
  { start: '13:00', end: '13:08', seats: 4, start_loc: 'Stefan Dressler' },
  { start: '12:15', end: '12:30', seats: 3, start_loc: 'Heizungstechnik' },
  { start: '14:00', end: '14:14', seats: 2, start_loc: 'Waldkircher Straße' },
  { start: '15:15', end: '15:19', seats: 5, start_loc: 'Opfingen' },
]

const selected = $ref(undefined)
const hover = $ref(undefined)

const img_src = computed(() => {
  if (hover !== undefined)
    return `map_${hover}.jpeg`

  if (selected !== undefined)

    return `map_${selected}.jpeg`

  else return 'map_empty.jpeg'
})

function get_color(id: number) {
  if (selected === id)
    return 'overwrite-color'

  else if (hover === id)
    return 'bg-gray-100'

  else
    return 'bg-white'
}
</script>

<template lang="pug">
div.h-screen.flex.flex-col.p-5
  h1 Suche dir eine Mitfahrgelegenheit

  div.flex.p-5
    div.card.p-5
      img.map_img(:src="img_src")
    div.self-right.flex.flex-col.p-5.flex-grow
      h2 Diese Fahrten stehen zur Verfügung
      div.style(
          v-for="(fahrt, index) in fahrten"
          :class="get_color(index)"
          @click="selected = index"
          @mouseover="hover = index"
          @mouseleave="hover = undefined"
          )
        div.flex
          span {{fahrt.start}}
          span.px-3 ->
          span {{fahrt.end}}

        div.flex
          span {{fahrt.start_loc}}
          span.px-3 ->
          span Opfinger See

        div.flex
          span {{fahrt.seats}}
          div(i="carbon-person")

      div.mt-5.flex.justify-end(v-if="selected !== undefined")
        router-link.rounded.p-5.book-button.text-white.text-2xl(to="success") Sitz buchen
</template>

<style lang="sass">
.style
  @apply flex justify-between mb-5 p-5 shadow-xl rounded border cursor-pointer

.overwrite-color
  background: rgb(22,163,74) !important
  color: white

.book-button
  background: rgb(22, 163, 74)

.card
  width: 65%

.map_img
  width: 100%

a
  text-decoration: none
  border: none
  color: black
</style>
