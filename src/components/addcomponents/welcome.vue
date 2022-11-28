<script>
export default {
  name: "welcome",
};
</script>

<template>
  <div class="welcome-class">
    <div class="container">
      <h1>welcome to fable</h1>
      <p>Lorem ipsum dolor sit amet.</p>
      <div class="card"></div>
      <div class="card"></div>
      <div class="card"></div>
      <div class="card"></div>
      <div class="container-gray">
        <div class="elements"></div>
        <div class="carousel-thumb"></div>
      </div>
    </div>
  </div>
</template>


<style lang="scss" scoped>
@use "../style/partial/variable" as *;
@use "../style/partial/mixin" as *;

.welcome-class {
  .container {
    @include centralFlex;
    flex-direction: column;
  }
}
</style>