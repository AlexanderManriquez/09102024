<!-- 4.-  Input de número con contador
Enunciado: Crea un componente que tenga un input de tipo número. El valor del input debe controlarse mediante v-model y mostrarlo en un párrafo. -->

<script>
export default {
  name: "Contador",
  data() {
    return {
        numero:""
    };
  },
};
</script>

<template>
  <div class="border">
    <input type="number" v-model="numero" placeholder="Ingresa un número"/>

    <p class="resultado">Tu número es: <span>{{ numero }}</span></p>
  </div>
</template>

<style>
    .border {
        border: 1px solid black;
        padding: 1rem;
        margin: 1rem;
    }

    .resultado {
        margin: 0;
        padding: 0;
    }

    span {
        color: red;
        font-weight: bold;
        font-size: 1.5rem;
    }
</style>
