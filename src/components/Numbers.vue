<!-- IMPORTA VARIABILI SASS -->

<script>
export default {};
</script>

<template>
  <div class="container">
    <div class="row justify-content-center">
      <div class="col-md-3">
        <div class="card text-center">
          <div class="card-body">
            <h5 class="card-title">Card 1</h5>
            <p class="card-number">1234</p>
            <p class="card-subtitle">Subtitle 1</p>
          </div>
        </div>
      </div>
      <div class="col-md-3">
        <div class="card text-center">
          <div class="card-body">
            <h5 class="card-title">Card 2</h5>
            <p class="card-number">5678</p>
            <p class="card-subtitle">Subtitle 2</p>
          </div>
        </div>
      </div>
      <div class="col-md-3">
        <div class="card text-center">
          <div class="card-body">
            <h5 class="card-title">Card 3</h5>
            <p class="card-number">9876</p>
            <p class="card-subtitle">Subtitle 3</p>
          </div>
        </div>
      </div>
      <div class="col-md-3">
        <div class="card text-center">
          <div class="card-body">
            <h5 class="card-title">Card 4</h5>
            <p class="card-number">5432</p>
            <p class="card-subtitle">Subtitle 4</p>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<style scoped>
.card {
  margin-top: 20px;
  border-radius: 10px;
  box-shadow: 0 2px 4px rgba(0, 0, 0, 0.1);
}

.card-title {
  font-size: 24px;
  font-weight: bold;
}

.card-number {
  font-size: 36px;
  font-weight: bold;
  color: #007bff; /* Change the color to your preference */
  margin-top: 10px;
}

.card-subtitle {
  font-size: 14px;
  color: #777;
  margin-top: 10px;
}
</style>
