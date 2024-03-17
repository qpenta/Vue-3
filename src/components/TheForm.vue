<template>
  <h2>Meu formulário:</h2>

  <form action="" @submit="enviarFormulario">
    <div>
      <input type="text" v-model="name" />
    </div>

    <div>
      <input type="text" v-model="email" />
    </div>
    <div>
      <TheSubmit />
    </div>
  </form>
  <p>Conteúdo</p>
  <p>Conteúdo</p>
  <p>Conteúdo</p>
</template>

<script>
import TheSubmit from "./Form/TheSubmit";

export default {
  name: "TheForm",
  components: {
    TheSubmit,
  },

  data() {
    return {
      name: "Yago",
      email: "test@gmail.com",
    };
  },
  methods: {
    enviarFormulario(e) {
      e.preventDefault();

      const name = this.name;
      const email = this.email;

      console.log("Forumulário Enviado!");
      console.log("O nome é:" + name);
      console.log("O email é:" + email);

      // Ajax

      // Inserir no banco de dados
    },
  },
};
</script>

<style>
p {
  margin: 50px;
}
</style>
