<!-- IMPORTA VARIABILI SASS -->

<script>
export default {};
</script>

<template>
  <section class="hero">
    <div class="container">
      <div class="row align-items-center">
        <!-- Left Column -->
        <div class="col-md-4">
          <div class="hero-content">
            <h1 class="hero-title">Title 1 Title 1 Title 1 Title 1</h1>
            <p class="hero-paragraph">
              Lorem ipsum, dolor sit amet consectetur adipisicing elit. Vel
              doloribus delectus consectetur,
            </p>
            <a href="#" class="btn">Learn More</a>
            <p class="hero-small-paragraph">Lorem ipsum, dolor sit amet</p>
          </div>
        </div>

        <!-- Right Column -->
        <div class="col-md-6 offset-md-2">
          <div class="hero-image-container">
            <div class="background-1">
              <img src="../assets/img/maxcoach-shape-02.png" alt="" />
            </div>
            <div class="background-2">
              <img src="../assets/img/maxcoach-shape-07-150x150.png" alt="" />
            </div>
            <div class="background-3">
              <img src="../assets/img/maxcoach-shape-08.png" alt="" />
            </div>
            <div class="background-4">
              <img src="../assets/img/maxcoach-shape-08.png" alt="" />
            </div>
            <div class="hero-image">
              <!-- Add your round-bordered image here -->
              <img
                src="../assets/img/about-me-profile-ohm4dxoearqbxny7q3bq1pzbdgofdx0tobbeqcvzd0.jpg"
                alt="Your Image"
                class="img-fluid rounded-circle"
              />
            </div>
          </div>
        </div>
      </div>
    </div>
    <div class="container">
      <div class="row justify-content-center">
        <div class="col-2">
          <img
            class="img-client"
            src="../assets/img/client-logo-01.png"
            alt=""
          />
        </div>
        <div class="col-2">
          <img
            class="img-client"
            src="../assets/img/client-logo-02.png"
            alt=""
          />
        </div>
        <div class="col-2">
          <img
            class="img-client"
            src="../assets/img/client-logo-03.png"
            alt=""
          />
        </div>
        <div class="col-2">
          <img
            class="img-client"
            src="../assets/img/client-logo-04.png"
            alt=""
          />
        </div>
        <div class="col-2">
          <img
            class="img-client"
            src="../assets/img/client-logo-05.png"
            alt=""
          />
        </div>
        <div class="col-2">
          <img
            class="img-client"
            src="../assets/img/client-logo-06.png"
            alt=""
          />
        </div>
      </div>
    </div>
  </section>
</template>

<style lang="scss" scoped>
@import "../styles/partials/variables";
.hero {
  padding: 100px 0;
  background-color: #ffffff;
  z-index: 0;
}

.hero-title {
  font-size: 36px;
  font-weight: bold;
}

.hero-paragraph {
  font-size: 18px;
  margin-top: 20px;
}

.btn {
  background-color: $button-bg-color;
  color: $button-text-color;
  font-size: $button-font-size;
  font-weight: $button-font-weight;
  border: $button-border;
}

.hero-small-paragraph {
  font-size: 14px;
  margin-top: 20px;
}

.hero-image {
  text-align: center;
}

.img-fluid.rounded-circle {
  border-radius: 50%;
  max-width: 100%;
  height: 500px;
}

.background-1,
.background-2,
.background-3,
.background-4 {
  position: absolute;
  width: 50%;
  height: 50%;
}

.img-client {
  margin-top: 10rem;
  opacity: 0.3;

  &:hover {
    opacity: 1;
  }
}
</style>
