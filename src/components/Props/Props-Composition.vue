<template>
  <div>
    <h4>Props Composition</h4>
    {{ fullName }}
  </div>
  <hr />
</template>

<script setup>
import { computed, defineProps, toRefs } from "vue";
const props = defineProps({
  firstName: String,
  lastName: String,
});

const { firstName, lastName } = toRefs(props);

const fullName = computed(() => {
  return `${firstName.value} ${lastName.value}`;
});
</script>
