<script>
import "swiper/css";

export default {
  name: "Jumbotron",
};
</script>

<template>
  <!-- il jumbo è a tutta pagina in larghezza, all'interno c'è un carosello con delle icone personalizzate e sotto ha un altra striscia con un bottone "learn more" che sono contenuti nel container -->
  <div class="jumbo-container">
    <div class="carousel">
      <img
        class="middle-img"
        src="../assets/img/slider_slide3_img2.png"
        alt=""
      />
      <img class="end-img" src="../assets/img/slider_slide3_img3.png" alt="" />
    </div>
    <div class="learn-more">
      <div class="container">
        <h1>How to Enroll Your Child to a Class?</h1>
        <button>learn more</button>
      </div>
    </div>
  </div>
</template>


<style lang="scss" scoped>
@use "../style/partial/variable" as *;
@use "../style/partial/mixin" as *;

.carousel {
  position: relative;
  width: 100%;
  background-image: url("../assets/img/slider_slide1_background.png");
  height: 600px;
  img {
    width: 250px;
    height: auto;
    .middle-img {
      position: absolute;
      bottom: 0;
      right: 100px;
    }
    .end-img {
      position: absolute;
      top: 0;
      left: 100px;
    }
  }
}
.learn-more {
  @include centralFlex("horizontal");
  height: 135px;
  background-image: url("../assets/img/pattern.png");
  .container {
    display: flex;
    justify-content: space-between;
    align-items: center;
    h1 {
      color: white;
    }
    button {
      padding: 5px 10px;
      color: white;
      border: 3px solid white;
      background-color: transparent;
      text-transform: uppercase;
    }
  }
}
</style>