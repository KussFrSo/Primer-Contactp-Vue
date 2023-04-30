<template>
  <div>
    <h4>Watch Composition</h4>
    <div>{{ obj }}</div>
    <div>{{ counter }}</div>
  </div>
  <hr />
</template>

<script setup>
import { reactive, ref, watch } from "vue";

//Opcion con un OBJ usando reactive
const obj = reactive({ counter: 0 });

// watch(
//   () => obj.counter,
//   (valorAnterior, valorNuevo) => {
//     console.log(valorAnterior, valorNuevo);
//   }
// );

//Opcion con una variable usando ref
const counter = ref(0);

watch(counter, (valorAnterior, valorNuevo) => {
  console.log(valorAnterior, valorNuevo);
});

/* ************************************ */

setInterval(() => {
  obj.counter++;
  counter.value++;
}, 500);
</script>
