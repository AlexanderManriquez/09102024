<!-- 6.-  Enlace dinámico al atributo href de un enlace
Enunciado: Crea un componente que tenga un enlace (a) donde el href sea dinámico. El valor del enlace debe estar en el data del componente y cambiarse mediante v-bind. -->

<script>
export default {
  name: "HrefDinamico",
  data() {
    return {
        href: ""
    };
  },
};
</script>

<template>
  <div class="border flex">
    <label>Elige un enlace:</label>
    <br>
    <select v-model="href">
      <option value="" selected disabled>Selecciona un enlace para visitar</option>
      <option value="http://www.google.com">Google</option>
      <option value="http://www.youtube.com">YouTube</option>
      <option value="http://www.facebook.com">Facebook</option>
      <option value="http://www.linkedin.com">LinkedIn</option>
    </select>
    <br>
    <a :href="href" target="_blank">Enlace mágico</a>
  </div>
</template>

<style>
    .flex {
        display: flex;
        flex-direction: column;
    }
</style>