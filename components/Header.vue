<script lang="ts">
export default {
  setup() {
    const count = ref(0);
    return { count };
  },
};
</script>

<template>
  <h1>header</h1>

  <button
    @click="
      () => {
        count++;
      }
    "
  >
    click
  </button>
  <div>count : {{ count }}</div>
</template>

<style scoped>
h1 {
  color: red;
  font-size: 18px;
  font-weight: bold;
}
</style>
