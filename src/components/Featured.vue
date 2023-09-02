<!-- IMPORTA VARIABILI SASS -->

<script>
export default {};
</script>

<template>
  <div class="my-container">
    <div class="d-flex col-12 flex-column align-items-center pt-5">
      <h5>STIMULATED TO LEARN ?</h5>
      <h2>Featured Online Courses</h2>
    </div>
    <div class="container">
      <div class="row">
        <!-- COL 1 -->
        <div class="col-md-6">
          <div class="row">
            <div class="col-4">
              <div class="round-image">
                <img
                  src="../assets/img/course-02-480x298.jpg"
                  alt="Image 1"
                  class="img-fluid rounded-circle"
                />
              </div>
            </div>
            <div class="col-8">
              <p class="price">$99</p>
              <h4 class="main-title">Main Title</h4>
              <span class="span">Span 1</span>
              <span class="span">Span 2</span>
            </div>
          </div>
        </div>
        <!-- COL 2 -->
        <div class="col-md-6">
          <div class="row">
            <div class="col-4">
              <div class="round-image">
                <img
                  src="../assets/img/course-02-480x298.jpg"
                  alt="Image 1"
                  class="img-fluid rounded-circle"
                />
              </div>
            </div>
            <div class="col-8">
              <p class="price">$99</p>
              <h4 class="main-title">Main Title</h4>
              <span class="span">Span 1</span>
              <span class="span">Span 2</span>
            </div>
          </div>
        </div>
      </div>
    </div>

    <!-- BOTTONE -->
    <div class="text-center mt-4">
      <button class="btn">Click Me</button>
    </div>
  </div>
</template>

<style lang="scss" scoped>
@import "../styles/partials/variables";

.my-container {
  background-color: rgb(245, 247, 250);
}
.container {
  padding: 40px;
  padding: 10rem 2rem;
}

.round-image {
  text-align: center;
  margin-bottom: 20px;
}

.rounded-circle {
  object-fit: cover;
  width: 150px;
  height: 150px;
  border-radius: 50%;
}

.main-title {
  font-size: 1.2rem;
  font-weight: 700;
  color: rgb(63, 58, 100);
}

.price {
  font-size: 1.3rem;
  font-weight: 700;
  color: rgb(32, 173, 150);
}

.span {
  font-weight: 700;
  font-size: 0.8rem;
  color: rgb(177, 177, 177);
}

.btn {
  background-color: $button-bg-color;
  color: $button-text-color;
  font-size: $button-font-size;
  font-weight: $button-font-weight;
  border: $button-border;
}

h2 {
  color: rgb(63, 58, 100);
}

h5 {
  font-weight: 700;
  font-size: 0.8rem;
  color: rgb(177, 177, 177);
  letter-spacing: 2px;
}
</style>
