<script>
import AppHeader from "./components/AppHeader.vue";
import Jumbotron from "./components/Jumbotron.vue";
import AppMain from "./components/AppMain.vue";
import AppFooter from "./components/AppMain.vue";

export default {
  name: "App",
  components: {
    AppHeader,
    Jumbotron,
    AppMain,
    AppFooter,
  },
};
</script>

<template>
  <AppHeader />
  <Jumbotron />
  <AppMain />
  <AppFooter />
</template>


<style lang="scss" scoped>
@use "./style/general";
</style>