<script setup>
  import Dropdown from './components/Dropdown.vue'
  import Contador from './components/Contador.vue'
  import HrefDinamico from './components/HrefDinamico.vue'
  import ClaseDinamica from './components/ClaseDinamica.vue'
</script>

<template>
  <Dropdown/>
  <Contador/>
  <HrefDinamico/>
  <ClaseDinamica/>
</template>

<style scoped>
.logo {
  height: 6em;
  padding: 1.5em;
  will-change: filter;
  transition: filter 300ms;
}
.logo:hover {
  filter: drop-shadow(0 0 2em #646cffaa);
}
.logo.vue:hover {
  filter: drop-shadow(0 0 2em #42b883aa);
}
</style>
