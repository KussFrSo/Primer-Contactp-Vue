<template>
  <div>
    <h4>Refs Options</h4>
    <button ref="btn">Click Me!</button>
  </div>
  <hr />
</template>

<script>
export default {
  mounted() {
    console.log(this.$refs.btn);
  },
};
</script>
