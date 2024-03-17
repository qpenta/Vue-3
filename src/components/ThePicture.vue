<template>
  <img :src="avatar" :alt="descricao" />
  <MudarImagem @mudar-imagem="trocarImagem" />
</template>

<script>
// import TheReutilizacao from "./TheReutilizacao";
import MudarImagem from "./MudarImagem.vue";

export default {
  name: "ThePicture",
  components: {
    // TheReutilizacao,
    MudarImagem,
  },
  data() {
    return {
      avatar: "/img/avatar.png",
      descricao: "Yago Batista",
    };
  },
  methods: {
    trocarImagem() {
      this.avatar = "/img/avatar2.png";
    },
  },
};
</script>

<style>
img {
  max-width: 200px;
}
</style>
