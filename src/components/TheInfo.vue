<template>
  <div>
    <p v-if="esta_trabalhando">Estou trabalhando no momento.</p>
    <p v-else>Estou em busca de novas oportunidades</p>
    <p>Utilizo as seguintes tecnologias:</p>

    <ul>
      <li>JavaScript</li>
      <li>Php</li>
      <li>Python</li>
    </ul>
    <div>
      <button @click="showEmail">{{ textoBotao }}</button>
    </div>
    <p v-show="mostrar_email">Mande uma mensagem para: {{ email }}</p>
    <p class="teste">
      Para acessar meu portifólio
      <a v-bind:href="meu_link" target="_blank">Basta clicar aqui</a>
    </p>
    <ThePicture />
  </div>
</template>

<script>
import ThePicture from "./ThePicture.vue";

export default {
  name: "TheInfo",
  components: {
    ThePicture,
  },
  data() {
    return {
      esta_trabalhando: false,
      mostrar_email: false,
      email: "teste@gmail.com",
      meu_link: "http://google.com",
      textoBotao: "Mostrar e-mail",
    };
  },
  methods: {
    showEmail() {
      this.mostrar_email = !this.mostrar_email;
      if (!this.mostrar_email) {
        this.textoBotao = "Mostrar e-mail";
      } else {
        this.textoBotao = "Esconder e-mail";
      }
    },
  },
};
</script>

<style>
.paragrafo-pai {
  color: red;
}
</style>
