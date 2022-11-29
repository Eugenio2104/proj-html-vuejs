<script>
export default {
  name: "AppFooter",
};
</script>
<template>
  <footer>
    <div class="container">
      <div class="row">
        <ul>
          <li>
            <h5><a href="#">about us</a></h5>
            <p>
              Lorem ipsum, dolor sit amet consectetur adipisicing elit. Et sit
              magnam facilis iure incidunt ex quidem cupiditate doloremque
              voluptas sint.
            </p>
            <img src="../assets/img/logo_footer.png" alt="" />
          </li>
          <li>
            <h5><a href="#">archives</a></h5>

            <button class="col-12">october 2014(2)</button>
            <button class="col-12">september 2014(2)</button>
            <button class="col-12">august 2014</button>
            <button class="col-12">july 2014(2)</button>
            <button class="col-12">june 2014(2)</button>
            <button class="col-12">may 2014(1)</button>
          </li>
          <li>
            <h5><a href="#">our features</a></h5>

            <p>
              Lorem ipsum, dolor sit amet consectetur adipisicing elit. Et sit
              magnam facilis iure incidunt ex quidem cupiditate doloremque
              voluptas sint.
            </p>
            <span>
              <i class="fa-regular fa-square-check"></i>
              firendly and welcoming place
            </span>
          </li>
          <li>
            <h5><a href="#">recent posts</a></h5>

            <p>
              Lorem ipsum, dolor sit amet consectetur adipisicing elit. Et sit
              magnam facilis iure incidunt ex quidem cupiditate doloremque
              voluptas sint.
            </p>
            <img src="../assets/img/logo_footer.png" alt="" />
          </li>
        </ul>
      </div>
    </div>
  </footer>
</template>
<style lang="scss" scoped>
@use "../style/partial/variable" as *;
@use "../style/partial/mixin" as *;
footer {
  margin-top: 150px;
  width: 100%;
  height: 400px;
  background-image: url("../assets/img/pattern.png");
  background-size: cover;
  .container {
    color: rgba(255, 255, 255, 0.304);
    ul {
      @include centralFlex("horizontal");
      justify-content: space-around;

      li {
        list-style: none;
        margin: 50px;
        flex-direction: column;
        h5 {
          font-weight: bold;
          text-transform: uppercase;
        }

        a {
          text-decoration: none;
          color: rgba(255, 255, 255, 0.304);
        }
        p {
          font-size: 0.8rem;
        }
        img {
          width: 150px;
        }
        button {
          margin-top: 7px;
          background-color: transparent;
          border: 2px solid rgba(255, 255, 255, 0.304);
          text-align: start;
          color: rgba(255, 255, 255, 0.304);
        }
      }
    }
  }
}
</style>