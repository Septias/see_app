<script lang="ts" setup>
const route = useRoute()
const router = useRouter()
const id = parseInt(route.fullPath[route.fullPath.length - 1])

document.addEventListener('keydown', (e) => {
  if (e.key === 'ArrowLeft')
    router.push(`/slide${id - 1}`)

  else if (e.key === 'ArrowRight')
    router.push(`/slide${id + 1}`)
})
</script>

<template lang="pug">
slot
</template>
