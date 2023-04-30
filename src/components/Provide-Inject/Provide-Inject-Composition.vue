<template>
  <div>
    <h4>Provide Inject Composition</h4>
    {{ appName }}
  </div>
  <hr />
</template>

<script setup>
import { inject, provide, ref } from "vue";

const appName = inject("appName");

const language = ref("es");
provide("language", language);
</script>
