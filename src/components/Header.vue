<template>
  <header>
    <div class="container">
      <div class="row">
        <div class="col-2"><img src="../assets/img/dc-logo.png" alt="" /></div>
        <div class="col-8">
          <ul>
            <li v-for="link in linkList" :key="link">
              <a :href="link.url">{{ link.text }}</a>
            </li>
          </ul>
        </div>
      </div>
    </div>
  </header>
</template>

<script>
export default {
  name: 'Header',
  data() {
    return {
      linkList: [
        {
          text: 'Characters',
          url: '#',
          current: false,
        },
        {
          text: 'Comics',
          url: '#',
          current: true,
        },
        {
          text: 'Movies',
          url: '#',
          current: false,
        },
        {
          text: 'TV',
          url: '#',
          current: false,
        },
        {
          text: 'Games',
          url: '#',
          current: false,
        },
        {
          text: 'Collectibles',
          url: '#',
          current: false,
        },
        {
          text: 'Videos',
          url: '#',
          current: false,
        },
        {
          text: 'Fans',
          url: '#',
          current: false,
        },
        {
          text: 'News',
          url: '#',
          current: false,
        },
        {
          text: 'Shop',
          url: '#',
          current: false,
        },
      ],
    };
  },
};
</script>

<style scoped>
header {
  height: 120px;
  width: 100%;
}

.col-8 {
  display: flex;
  justify-content: end;
  align-items: center;
}

ul {
  display: flex;
  align-items: center;
}
ul li {
  margin-right: 20px;
  list-style: none;
}

ul li a {
  text-transform: uppercase;
  text-decoration: none;
  font-size: 0.8rem;
  color: gray;
}
</style>
