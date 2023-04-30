<template>
  <div>
    <h4>Refs Composition</h4>
    <button ref="btn">Click Me!</button>
  </div>
  <hr />
</template>

<script setup>
import { ref, watch } from "vue";

const btn = ref(null);

watch(btn, (valor) => {
  console.log(valor);
});
</script>
