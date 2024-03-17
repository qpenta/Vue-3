<template>
  <div>
    <h1>Olá vue</h1>
    <p>Meu nome é {{ nome }} e trabalho como {{ profissao }}</p>
    <MultiplosEventos />
    <TheReutilizacao />
    <TheReutilizacao />
    <TheReutilizacao />
  </div>
</template>

<script>
import MultiplosEventos from "./MultiplosEventos";
import TheReutilizacao from "./TheReutilizacao";

export default {
  name: "PrimeiroComponente",
  components: {
    MultiplosEventos,
    TheReutilizacao,
  },
  data() {
    return {
      nome: "Yago",
      profissao: "Desenvolvedor",
    };
  },
};
</script>
