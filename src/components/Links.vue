<template>
  <section>
    <div class="container">
      <div class="row">
        <div class="col-4">
          <div class="list">
            <ul>
              <h3>dc comics</h3>
              <li v-for="link in linkList" :key="link">{{ link.text }}</li>
            </ul>
            <ul>
              <h3>Shop</h3>
              <li>Shop DC</li>
              <li>Shop DC Collectibles</li>
            </ul>
          </div>
          <div class="list">
            <ul>
              <h3>DC</h3>
              <li>Terms Of Use</li>
              <li>Privacy policy (New)</li>
              <li>Ad Choices</li>
              <li>Advertising</li>
              <li>Jobs</li>
              <li>Subscriptions</li>
              <li>Talent Workshops</li>
              <li>CPSC Certificates</li>
              <li>Ratings</li>
              <li>Shop Help</li>
              <li>Contact Us</li>
            </ul>
          </div>
          <div class="list">
            <ul>
              <h3>Sites</h3>
              <li>DC</li>
              <li>MAD Magazine</li>
              <li>DC Kids</li>
              <li>DC Universe</li>
              <li>DC Power Visa</li>
            </ul>
          </div>
        </div>
        <div class="col-6">
          <figure>
            <img src="../assets/img/dc-logo-bg.png" alt="" />
          </figure>
        </div>
      </div>
    </div>
  </section>
</template>

<script>
export default {
  name: 'Links',
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
section {
  width: 100%;
  height: 350px;
  background-image: url('../assets/img/footer-bg.jpg');
  background-size: cover;
  overflow: hidden;
}

figure {
  display: flex;
  justify-content: end;
}

img {
  width: 450px;
}

.col-4 {
  display: flex;
  justify-content: space-between;
}

.list {
  display: flex;
  flex-direction: column;
  justify-content: space-between;
}

ul li {
  list-style: none;
  color: gray;
  font-size: 0.7rem;
  margin-top: 3px;
}

h3 {
  margin-top: 10px;
  color: white;
  text-transform: uppercase;
  font-size: 1rem;
}
</style>
