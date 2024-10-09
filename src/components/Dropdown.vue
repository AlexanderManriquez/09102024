<!-- 2.-  Selección de opción en un dropdown
Enunciado: Crea un componente con un menú desplegable (select) que permita al usuario elegir una opción de color. Muestra el color seleccionado dinámicamente en un párrafo debajo. -->

<script>
export default {
  name: "Dropdown",
  data() {
    return {
      color: ""
    };
  },
};
</script>

<template>
  <div class="border">
    <select v-model="color">
      <option value="" selected disabled>Selecciona un color</option>
      <option value="yellow">Amarillo</option>
      <option value="red">Rojo</option>
      <option value="green">Verde</option>
      <option value="blue">Azul</option>
    </select>

    <p :style="{ backgroundColor: color }">Aquí te muestro el color</p>
  </div>
</template>

<style>
    p {
        padding: 1rem;
        border-radius: 1rem;
    }
</style>
