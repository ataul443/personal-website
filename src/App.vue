<template>
  <router-view v-bind:user="user"></router-view>
</template>

<script>
import HomePage from "./components/HomePage/HomePage";
export default {
  name: "App",
  components: {
    "home-page": HomePage
  },
  data: function data() {
    return {
      user: {
        name: "Shekh Ataul",
        role: "Backend Developer"
      }
    };
  }
};
</script>

<style>
html {
  font-size: 16px;
  width: 100vw;
  height: 100vh;
}
.columns {
  margin: 0;
}

@media screen and (min-width: 768px) {
  .columns {
    margin-left: -0.75rem;
    margin-right: -0.75rem;
    margin-top: -0.75rem;
  }
}
</style>
