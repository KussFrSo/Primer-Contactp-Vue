<template>
  <div>
    <h4>Computed Options</h4>
    {{ fullName }}
  </div>
  <hr />
</template>

<script>
export default {
  data() {
    return {
      firstName: "Marc",
      lastName: "Franch",
    };
  },
  computed: {
    fullName() {
      return `${this.firstName} ${this.lastName}`;
    },
  },
};
</script>
