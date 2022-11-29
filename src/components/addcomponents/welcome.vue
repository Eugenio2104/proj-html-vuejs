<script>
export default {
  name: "Welcome",
  data() {
    return {
      cardElements: [
        {
          img: "",
          color: "",
        },
        {
          img: "",
          color: "",
        },
        {
          img: "",
          color: "",
        },
        {
          img: "",
          color: "",
        },
      ],
    };
  },
};
</script>

<template>
  <div class="welcome-class">
    <div class="container">
      <h1>Welcome to fable</h1>
      <p>Fable daycare,preschool, and kindergarten</p>
      <img src="../../assets/img/header_divider.png" alt="" />
      <div class="card-container">
        <div class="eb-card col-1 offset-2"></div>
        <div class="eb-card col-1 offset-2"></div>
        <div class="eb-card col-1 offset-2"></div>
        <div class="eb-card col-1 offset-2"></div>
      </div>
    </div>
  </div>
</template>


<style lang="scss" scoped>
@use "../style/partial/variable" as *;
@use "../style/partial/mixin" as *;

.welcome-class {
  .container {
    margin-top: 40px;
    @include centralFlex;
    flex-direction: column;
    h1 {
      font-size: 3rem;
      color: $secondary-color;
      p {
        color: grey;
      }
    }
    img {
      width: 100px;
    }
    .card-container {
      @include centralFlex;
      .eb-card {
        background-image: url("../../assets/img/schoolbag_alt.png");
        background-size: 40px;
        background-position: center;
        background-repeat: no-repeat;
        background-color: $primary-color;

        margin-top: 50px;
        width: 120px;
        height: 120px;
        border-radius: 50%;
      }
    }
  }
}
</style>