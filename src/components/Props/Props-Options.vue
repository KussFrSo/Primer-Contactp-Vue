<template>
  <div>
    <h4>Props Options</h4>
    {{ fullName }}
  </div>
  <hr />
</template>

<script>
export default {
  props: {
    firstName: String,
    lastName: String,
  },
  computed: {
    fullName() {
      return `${this.firstName} ${this.lastName}`;
    },
  },
};
</script>
