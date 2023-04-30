<template>
  <div>
    <h4>Watch Options</h4>
    {{ counter }}
  </div>
  <hr />
</template>

<script>
export default {
  data() {
    return {
      counter: 0,
    };
  },
  watch: {
    // counter(valorNuevo, valorAnterior) {
    //   console.log(valorAnterior, valorNuevo);
    // },
  },
  created() {
    setInterval(() => this.counter++, 500);
  },
};
</script>
