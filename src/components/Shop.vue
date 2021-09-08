<template>
  <section>
    <div class="container">
      <div class="row">
        <ul>
          <li>
            <div class="product">
              <figure>
                <img
                  src="../assets/img/buy-comics-digital-comics.png"
                  width="50%"
                  alt=""
                />
              </figure>
              <span>digital comics</span>
            </div>
          </li>
          <li>
            <div class="product">
              <figure>
                <img
                  src="../assets/img/buy-comics-merchandise.png"
                  width="50%"
                  alt=""
                />
              </figure>
              <span>dc merchandise</span>
            </div>
          </li>
          <li>
            <div class="product">
              <figure>
                <img
                  src="../assets/img/buy-comics-subscriptions.png"
                  width="50%"
                  alt=""
                />
              </figure>
              <span>subscription</span>
            </div>
          </li>
          <li>
            <div class="product">
              <figure>
                <img
                  src="../assets/img/buy-comics-shop-locator.png"
                  width="50%"
                  alt=""
                />
              </figure>
              <span>comic shop locator</span>
            </div>
          </li>
          <li>
            <div class="product">
              <figure>
                <img
                  src="../assets/img/buy-dc-power-visa.svg"
                  width="50%"
                  alt=""
                />
              </figure>
              <span>dc power visa</span>
            </div>
          </li>
        </ul>
      </div>
    </div>
  </section>
</template>

<script>
export default {
  name: 'Shop',
};
</script>

<style scoped>
section {
  width: 100%;
  height: 200px;
  background-color: #0082f9;
}
span {
  text-transform: uppercase;
  font-size: 0.8rem;
  color: white;
}
ul {
  display: flex;
}
ul li {
  max-width: 15vw;
  list-style: none;
  display: flex;
  align-items: center;
  margin-right: 30px;
}

.product {
  display: flex;
  align-items: center;
}

.product figure {
  flex-basis: 30%;
}
</style>
