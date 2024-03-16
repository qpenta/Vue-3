<template>
  <img :src="avatar" :alt="descricao" />
</template>

<script>
export default {
  name: "ThePicture",
  data() {
    return {
      avatar: "/img/avatar.png",
      descricao: "Yago Batista",
    };
  },
};
</script>
