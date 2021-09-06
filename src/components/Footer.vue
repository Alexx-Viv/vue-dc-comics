<template>
  <section>
    <div class="container">
      <div class="row">
        <div class="col-2">
          <div class="button">sign-up now!</div>
        </div>
        <div class="col-8">
          <span>Follow Us</span>
          <img src="../assets/img/footer-facebook.png" alt="" />
          <img src="../assets/img/footer-twitter.png" alt="" />
          <img src="../assets/img/footer-youtube.png" alt="" />
          <img src="../assets/img/footer-pinterest.png" alt="" />
          <img src="../assets/img/footer-periscope.png" alt="" />
        </div>
      </div>
    </div>
  </section>
</template>

<script>
export default {
  name: 'Footer',
};
</script>

<style scoped>
section {
  width: 100%;
  height: 100px;
  background-color: #303030;
}

.button {
  width: fit-content;
  padding: 10px 15px;
  text-transform: uppercase;
  color: white;
  border: 2px solid #0082f9;
}

.col-8 {
  display: flex;
  justify-content: end;
  align-items: center;
}

img {
  margin-right: 10px;
}

span {
  text-transform: uppercase;
  color: #0082f9;
  margin-right: 10px;
}
</style>
