<template>
  <NavBar :logo="logo_src" :alt="app_name" />
  <router-view />
  <TheFooter />
</template>

<script>
import NavBar from "./components/NavBar";
import TheFooter from "./components/TheFooter";

export default {
  components: {
    TheFooter,
    NavBar,
  },
  data() {
    return {
      logo_src: "/img/logo.png",
      app_name: "Make your burger",
    };
  },
};
</script>
<style>
* {
  font-family: Helvetica;
  padding: 0;
  margin: 0;
  box-sizing: border-box;
}

.main-container {
  margin: 50px;
  min-height: 0px;
}

h1 {
  text-align: center;
  font-size: 42px;
  margin-bottom: 40px;
  color: #222;
}
</style>
