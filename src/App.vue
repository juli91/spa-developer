<template>
  <div id="app">
    <div class="container">
      <Header />
      <Main />
    </div>
    <Footer />
  </div>
</template>

<script>
import Header from "./components/Header.vue";
import Main from "./components/Main.vue";
import Footer from "./components/Footer.vue";

export default {
  name: "App",
  components: {
    Header,
    Main,
    Footer,
  },
};
</script>

<style lang="scss">
@import url("https://fonts.googleapis.com/css2?family=Space+Grotesk:wght@500;700&display=swap");

:root {
  --primary: #151515;
  --highlighted: #4ee1a0;
  --dark-grey: #242424;
  --secondary: #ffffff;
  --text-color: #d9d9d9;
  --h1-font-size: 88px;
  --h2-font-size: 48px;
  --h3-font-size: 24px;
  --h1-letter-spacing: -2.5px;
  --h2-letter-spacing: -1.5px;
}

body {
  background-color: var(--primary);
}

#app {
  font-family: "Space Grotesk", sans-serif;
  font-size: 18px;
  line-height: 1.75;
  margin: 0;
  color: var(--text-color);

  h1,
  h2,
  h3,
  aside {
    color: var(--secondary);
    font-weight: bold;
  }

  h1 {
    font-size: var(--h1-font-size);
  }

  h2 {
    font-size: var(--h2-font-size);
  }

  h3 {
    font-size: var(--h3-font-size);
  }

  button {
    border: none;
    background: transparent;
    color: var(--secondary);
    text-decoration: underline var(--highlighted);
    text-transform: uppercase;

    &:hover {
      color: var(--highlighted);
    }
  }
}
</style>
