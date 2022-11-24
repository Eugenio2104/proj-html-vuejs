<script>
export default {
  name: "Jumbotron",
};
</script>

<template>
  <!-- il jumbo è a tutta pagina in larghezza, all'interno c'è un carosello con delle icone personalizzate e sotto ha un altra striscia con un bottone "learn more" che sono contenuti nel container -->
  <div class="jumbo-container">
    <div class="carousel"></div>
    <div class="learn-more">
      <div class="container">
        <h1>Lorem ipsum dolor sit amet.</h1>
        <button>learn more</button>
      </div>
    </div>
  </div>
</template>


<style lang="scss" scoped>
.carousel {
  width: 100%;
  background-color: grey;
  height: 600px;
}
.learn-more {
  height: 135px;
  background-color: purple;
  .container {
    display: flex;
    justify-content: space-between;
    align-items: center;
  }
}
</style>