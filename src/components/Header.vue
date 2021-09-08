<template>
  <header>
    <div class="container">
      <div class="row">
        <div class="col-2"><img src="../assets/img/dc-logo.png" alt="" /></div>
        <div class="col-8">
          <ul>
            <li
              v-for="link in linkList"
              :key="link"
              :class="{ active: link.current }"
            >
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
  height: 100%;
}

ul {
  display: flex;
  align-items: center;
  height: 100%;
}
ul li {
  padding: 0 10px;
  list-style: none;
  height: 100%;
  display: flex;
  align-items: center;
}
ul li:hover {
  background-color: lightgray;
  border-bottom: 4px solid #0082f9;
  cursor: pointer;
}

ul li.active {
  border-bottom: 4px solid #0082f9;
  background-color: lightgray;
}

ul li a {
  text-transform: uppercase;
  text-decoration: none;
  font-size: 0.8rem;
  color: gray;
}
</style>
