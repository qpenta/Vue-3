<template>
  <div>
    <TheHeader :esta_logado="true" />
    <PrimeiroComponente />
    <p class="paragrafo-pai">O dado de app é: {{ testando }}</p>
    <LifeCycle />
    <ThePessoa />
  </div>
</template>

<script>
import TheHeader from "./components/TheHeader.vue";
import PrimeiroComponente from "./components/PrimeiroComponente.vue";
import LifeCycle from "./components/LifeCycle.vue";
import ThePessoa from "./components/ThePessoa.vue";

export default {
  name: "App",
  components: {
    TheHeader,
    PrimeiroComponente,
    LifeCycle,
    ThePessoa,
  },
  data() {
    return {
      testando: "Teste",
    };
  },
};
</script>

<style>
body {
  background-color: #333;
  color: #fff;
}

a {
  color: red;
}

.teste {
  background: #000;
}
</style>
