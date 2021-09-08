<template>
  <section>
    <div class="container">
      <div class="card" v-for="comic in DcComics" :key="comic">
        <figure>
          <img :src="comic.thumb" :alt="comic.series" />
          <figcaption>{{ comic.series }}</figcaption>
        </figure>
      </div>
    </div>
    <div class="button">Load More</div>
  </section>
</template>

<script>
import DcComics from '../data/dc-comics.js';
export default {
  name: 'Content',
  data() {
    return {
      DcComics,
    };
  },
};
</script>

<style scoped>
section {
  width: 100%;
  height: 100%;
  background-color: black;
  display: flex;
  flex-direction: column;
  align-items: center;
  padding-bottom: 5vh;
}

.container {
  height: 100%;
  max-width: 1200px;
  display: flex;
  align-items: center;
  flex-wrap: wrap;
}
.card {
  flex-basis: calc(100% / 6);
  margin: 5vh;
}
figcaption {
  margin-top: 2vh;
  color: white;
}

.button {
  background-color: #0082f9;
  color: white;
  padding: 10px 25px;
  cursor: pointer;
}
.button:hover {
  background-color: white;
  color: #0082f9;
}
</style>
