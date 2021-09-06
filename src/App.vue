<template>
  <div id="app">
    <Header />
    <main>
      <Content />
      <Shop />
      <Links />
    </main>
    <Footer />
  </div>
</template>

<script>
import Header from './components/Header.vue';
import Content from './components/Content.vue';
import Shop from './components/Shop.vue';
import Links from './components/Links.vue';
import Footer from './components/Footer.vue';

export default {
  name: 'App',
  components: {
    Header,
    Content,
    Shop,
    Links,
    Footer,
  },
};
</script>

<style lang="scss">
* {
  box-sizing: border-box;
  padding: 0;
  margin: 0;
}

body {
  font-family: sans-serif;
}

img {
  max-width: 100%;
  height: auto;
}

.container {
  height: 100%;
  max-width: 1200px;
  margin: 0 auto;
}

.row {
  align-items: center;
  height: 100%;
  display: flex;
}

.col-2 {
  width: 20%;
}
.col-4 {
  width: 40%;
}
.col-6 {
  width: 60%;
}

.col-8 {
  width: 80%;
}
</style>
