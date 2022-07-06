<template lang="pug">
div.h-screen.flex.justify-center.items-center
  div.flex.flex-col
    h1 Auf zum See!
    p Schaue dir hier die aktuell angebotenen Mitfahrgelegenheiten zum Opfinger See an
    div.flex.justify-center
      router-link(to="view").p-5.bg-green-600.rounded.text-white.text-xl.m-10 Mitfahren
</template>
