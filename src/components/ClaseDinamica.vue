<!-- 8.-  Clases dinámicas con v-bind:class
Enunciado: Crea un componente que tenga un botón. El botón debe tener una clase CSS dinámica que cambie según un valor booleano en el data. Usa v-bind:class para aplicar la clase condicionalmente. -->

<script>
export default {
  name: "ClaseDinamica",
  data() {
    return {
        href: ""
    };
  },
};
</script>

<template>
  <div class="border">
    <button class="">Presiona aquí</button>
  </div>
</template>

<style>

</style>