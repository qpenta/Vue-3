<template>
  <div>
    <button @click="ativar">Clique Aqui!</button>
    <span v-show="ativou">Ativado!</span>
  </div>
</template>

<script>
export default {
  name: "TheReutilizacao",
  data() {
    return {
      ativou: false,
    };
  },
  methods: {
    ativar() {
      this.ativou = !this.ativou;
    },
  },
};
</script>
