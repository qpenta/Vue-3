<template>
  <TheBanner />
  <div class="main-container"></div>
  <h1>Monte o seu Burger:</h1>
  <BurgerForm />
</template>

<script>
import TheBanner from "/src/components/TheBanner.vue";
import BurgerForm from "/src/components/BurgerForm.vue";

export default {
  name: "TheHome",
  components: {
    TheBanner,
    BurgerForm,
  },
};
</script>
