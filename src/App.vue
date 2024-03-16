<template>
  <div>
    <PrimeiroComponente />
    <p>O dado de app é: {{ testando }}</p>
    <LifeCycle />
    <ThePessoa />
  </div>
</template>

<script>
import PrimeiroComponente from "./components/PrimeiroComponente.vue";
import LifeCycle from "./components/LifeCycle.vue";
import ThePessoa from "./components/ThePessoa.vue";

export default {
  name: "App",
  components: {
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
