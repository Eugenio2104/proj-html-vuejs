<script>
export default {
  name: "AppHeader",
};
</script>

<template>
  <header>
    <div class="container">
      <div class="logo">
        <h1>LOGO</h1>
      </div>
      <nav>
        <ul>
          <li>LI</li>
          <li>LI</li>
          <li>LI</li>
          <li>LI</li>
          <li>LI</li>
          <li>LI</li>
          <li>LI</li>
        </ul>
      </nav>
    </div>
  </header>
</template>


<style lang="scss" scoped>
@use "../style/partial/variable" as *;
@use "../style/partial/mixin" as *;
.container {
  height: 120px;
  @include centralFlex("vertical");
  @include centralFlex("space-between");
  nav {
    height: 100%;
    @include centralFlex;
    ul {
      @include centralFlex("horizontal");
    }
  }
}
</style>