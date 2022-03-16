<template>
  <div class="teste-if">
    <h1 v-if="podeVer">Positivo</h1>
    <h1 v-else>negativo</h1>
  </div>
</template>

<script>
export default {
  name: "testeIf",
  data() {
    return {
      podeVer: false,
    };
  },
};
</script>

<style scoped>
</style>