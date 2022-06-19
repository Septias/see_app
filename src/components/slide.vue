<script lang="ts" setup>
const route = useRoute()
const router = useRouter()
const id = parseInt(route.name.substring(5))

const listener = (e: any) => {
  if (e.key === 'ArrowLeft')
    router.push(`/slide${id - 1}`)

  else if (e.key === 'ArrowRight')
    router.push(`/slide${id + 1}`)
}
document.addEventListener('keydown', listener)

onUnmounted(() => {
  document.removeEventListener('keydown', listener)
})
</script>

<template lang="pug">
slot
</template>
