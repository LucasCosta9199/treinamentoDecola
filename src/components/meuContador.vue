<template>
  <div class="meu-contador">
    <p><strong>Contador:</strong> {{ contador }}</p>
    <button @click="removerUm">-</button>
    <button @click="somarUm">+</button>
  </div>
</template>

<script>
export default {
  name: "meuContador",
  data() {
    return {
      contador: 0,
    };
  },
  methods: {
    somarUm() {
      this.contador++;
    },
    removerUm() {
      this.contador--;
    },
  },
};
</script>