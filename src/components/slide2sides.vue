<template lang="pug">
div.flex.flex-col
  .flex
    div(class="w-1/2 mr-2")
      slot(name="left")
    div(class="w-1/2 ml-2")
      slot(name="right")
</template>
