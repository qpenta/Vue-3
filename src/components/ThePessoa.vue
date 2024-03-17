<template>
  <h2>Esta é a descrição da pessoa: {{ nome }}</h2>
  <TheInfo :email="email" :esta_trabalhando="false" />
  <TheInfo />
  <TheForm />
</template>

<script>
import TheInfo from "./TheInfo";
import TheForm from "./TheForm";

export default {
  name: "ThePessoa",
  components: {
    TheInfo,
    TheForm,
  },
  data() {
    return {
      nome: "Yago",
      email: "yago@gmail.com",
    };
  },
};
</script>

<style>
img {
  max-width: 200px;
}
</style>
