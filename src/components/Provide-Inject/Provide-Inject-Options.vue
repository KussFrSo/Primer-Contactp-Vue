<template>
  <div>
    <h4>Provide Inject Options</h4>
    {{ appName }}
  </div>
  <hr />
</template>

<script>
export default {
  inject: ["appName"],
  data() {
    return {
      language: "es",
    };
  },
  provide() {
    return {
      language: this.language,
    };
  },
};
</script>
