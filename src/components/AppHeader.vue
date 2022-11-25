<script>
export default {
  name: "AppHeader",
  data() {
    return {
      iconHeader: [
        {
          image: "../assets/img/document (1).png",
          href: "#",
          text: "home",
          current: "active",
        },
        {
          image: "../assets/img/document (1).png",
          href: "#",
          text: "home",
          current: "false",
        },
        {
          image: "../assets/img/document (1).png",
          href: "#",
          text: "home",
          current: "false",
        },
        {
          image: "../assets/img/document (1).png",
          href: "#",
          text: "home",
          current: "false",
        },
        {
          image: "../assets/img/document (1).png",
          href: "#",
          text: "home",
          current: "false",
        },
        {
          image: "../assets/img/document (1).png",
          href: "#",
          text: "home",
          current: "false",
        },
        {
          image: "../assets/img/document (1).png",
          href: "#",
          text: "home",
          current: "false",
        },
      ],
    };
  },
};
</script>


<template>
  <!-- header dentro a un container come altri elementi del layout -->
  <header>
    <div class="container">
      <div class="logo">
        <img src="../assets/img/logo.png" alt="" />
      </div>
      <nav>
        <div v-for="(icon, index) in iconHeader" :key="index" class="icons">
          <a :href="icon.href" :class="{ active: icon.current == 'active' }">
            <img :src="icon.image" alt="" />
            <span> {{ icon.text }} </span>
          </a>
        </div>
      </nav>
    </div>
  </header>
</template>


<style lang="scss" scoped>
@use "../style/partial/variable" as *;
@use "../style/partial/mixin" as *;

.container {
  height: 120px;
  @include centralFlex("horizontal");
  @include centralFlex("space-between");
  .logo {
    img {
      width: 200px;
    }
  }
  nav {
    height: 100%;
    @include centralFlex;
    .icons {
      @include centralFlex("vertical");
      flex-direction: column;
      padding: 30px;
      background-image: url("../assets/img/home.png");
      a {
        text-decoration: none;
        &.active,
        &:hover {
          color: $secondary-color;
          background-color: $primary-color;
        }
        img {
          width: 40px;
        }
        span {
          text-transform: uppercase;
        }
      }
    }
  }
}
</style>