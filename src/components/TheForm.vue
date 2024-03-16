<template>
  <h2>Meu formulário:</h2>
  <form action="">
    <div>
      <InputText />
    </div>
    <div>
      <InputText />
    </div>
    <div>
      <TheSubmit />
    </div>
  </form>
</template>

<script>
import InputText from "./Form/InputText";
import TheSubmit from "./Form/TheSubmit";

export default {
  name: "TheForm",
  components: {
    InputText,
    TheSubmit,
  },
};
</script>
