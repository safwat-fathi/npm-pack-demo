<template>
  <img
    alt="Vue logo"
    src="./assets/logo.png"
  >
  <p>Lorem ipsum dolor sit amet consectetur, adipisicing elit. Voluptatibus sunt nobis, consequatur facilis iusto magni beatae maiores libero? Aliquam, fugit. Veniam asperiores explicabo possimus hic aut maxime atque cumque blanditiis illo laboriosam?</p>
</template>

<script>
import shortIt from "short-itt";

export default {
  name: "App",
  mounted() {
    shortIt("for your information", (err, resp) => {
      if (err) {
        console.log(err);
      }

      console.log(resp);
    });
  },
};
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
