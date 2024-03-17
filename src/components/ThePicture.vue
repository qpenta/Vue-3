<template>
  <img :src="avatar" :alt="descricao" />
  <TheReutilizacao />
</template>

<script>
import TheReutilizacao from "./TheReutilizacao";

export default {
  name: "ThePicture",
  components: {
    TheReutilizacao,
  },
  data() {
    return {
      avatar: "/img/avatar.png",
      descricao: "Yago Batista",
    };
  },
};
</script>
