<template>
  <div class="meu-contador">
    <p>Meu Contador {{ valor }}</p>
    <p v-on:click="aumentar">[AUMENTAR]</p>
    <p v-on:click="diminuir">[DIMINUIR]</p>
  </div>
</template>

<script>
export default {
  name: "desafioContador",
  data() {
    return {
      valor: 0
    };
  },
  methods: {
    aumentar() {
      this.dell = this.dell += 1 ;
    },
    diminuir() {
      this.dell = this.dell -= 1;
    },
  },
};
</script>