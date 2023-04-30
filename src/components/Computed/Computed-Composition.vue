<template>
  <div>
    <h4>Computed Composition</h4>
    {{ fullName }}
  </div>
  <hr />
</template>

<script setup>
import { ref, computed } from "vue";

const firstName = ref("Marc");
const lastName = ref("Franch");

const fullName = computed(() => {
  return `${firstName.value} ${lastName.value}`;
});
</script>
