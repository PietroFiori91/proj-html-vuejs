<!-- IMPORTA VARIABILI SASS -->

<script>
export default {};
</script>

<template>
  <div class="my-container">
    <div class="container py-5">
      <div class="row justify-content-center">
        <!-- UL DIV -->
        <div class="col-md-4">
          <h3>ENJOYABLE INSIGHTS</h3>
          <div class="container-box">
            <h1 class="title">Most Viewed <span>Best Blog</span></h1>
            <ul>
              <li><i class="fas fa-arrow-right"></i> Item 1</li>
              <li><i class="fas fa-arrow-right"></i> Item 2</li>
              <li><i class="fas fa-arrow-right"></i> Item 3</li>
              <li><i class="fas fa-arrow-right"></i> Item 1</li>
              <li><i class="fas fa-arrow-right"></i> Item 2</li>
            </ul>
          </div>
        </div>

        <!-- CARD 1 -->
        <div class="col-md-4">
          <div class="card container-box">
            <img
              src="../assets/img/artist-blog-03-480x352.jpeg"
              class="card-img-top"
              alt="Image 1"
            />
            <div class="card-body">
              <h5 class="card-title">Card Title 1</h5>
            </div>
          </div>
        </div>

        <!-- CARD 2 -->
        <div class="col-md-4">
          <div class="card container-box">
            <img
              src="../assets/img/artist-blog-01-480x352.jpg"
              class="card-img-top"
              alt="Image 2"
            />
            <div class="card-body">
              <h5 class="card-title">Card Title 2</h5>
            </div>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<style lang="scss" scoped>
h3 {
  font-size: 0.8rem;
  font-weight: 700;
  color: rgb(169, 166, 183);
  letter-spacing: 2px;
}
.title {
  font-size: 24px;
  margin-bottom: 10px;
  color: rgb(63, 58, 100);
}

span {
  color: rgb(32, 173, 150);
  font-weight: 400;
}

ul {
  list-style: none;
  padding: 0;
}

li {
  margin-bottom: 5px;
  color: rgb(63, 58, 100);
}

.card {
  border: none;
  background-color: white;
}

.card-title {
  font-size: 18px;
}

.fas {
  font-size: 0.7rem;
  padding-right: 0.8rem;
  color: rgb(63, 58, 100);
}

.my-container {
  background-color: rgb(245, 241, 237);
}
</style>
