<template>
  <div class="teste-for">
    <h1>Teste for</h1>
    <ul>
      <li v-for="animal of animais" v-bind:key="animal.id">
        <img v-bind:src="animal.url" v-bind:alt="animal.nome" />
      </li>
    </ul>
  </div>
</template>

<script>
export default {
  name: "testeFor",
  data() {
    return {
      animais: 
      [
        {
          id: 1,
          nome: "carro 1",
          url: "https://www.petz.com.br/blog/wp-content/uploads/2020/04/meu-primeiro-gato.jpg",
        },
        {
          id: 2,
          nome: "carro 2",
          url: 'https://image.cachorrogato.com.br/thumb/1200/630/1/imagens/original/imagem858.jpg',
        },
      ],
    };
  },
};
</script>