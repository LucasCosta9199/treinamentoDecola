<template>
  <div class="teste-evento">
    <h1>Evento usuário</h1>
    <p @click="deixarMaiuscula">{{ mensagem }}</p>
    <p>teste</p>
    <p>teste</p>
    <p>teste</p>
    <p>teste</p>
    <p @mouseover="deixarMin">{{ mensagem2 }}</p>
  </div>
</template>

<script>
export default {
  name: "testeEvento",
  data() {
    return {
      mensagem: "Quem vue, vue!",
      mensagem2: "QueM n/Vue, n/VuE!",
    };
  },
  methods: {
    deixarMaiuscula() {
      this.mensagem = this.mensagem.toUpperCase();
    },
    deixarMin() {
      this.mensagem2 = this.mensagem2.toLowerCase();
    },
  },
};
</script>

<style scoped>
</style>