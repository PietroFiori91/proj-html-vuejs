<!-- IMPORTA VARIABILI SASS -->
<!-- _______________________________ -->
<!-- DYNAMICALLY ADD NUMBERS -->

<script>
export default {};
</script>

<template>
  <div class="container">
    <div class="row">
      <div class="col-md-3">
        <div class="card border-right text-center">
          <div class="card-body py-5">
            <h5 class="card-title my-5">Card 1</h5>
            <p class="card-number">1234</p>
            <p class="card-subtitle mb-5">Subtitle 1</p>
          </div>
        </div>
      </div>
      <div class="col-md-3">
        <div class="card border-right text-center">
          <div class="card-body py-5">
            <h5 class="card-title my-5">Card 2</h5>
            <p class="card-number">5678</p>
            <p class="card-subtitle mb-5">Subtitle 2</p>
          </div>
        </div>
      </div>
      <div class="col-md-3">
        <div class="card border-right text-center">
          <div class="card-body py-5">
            <h5 class="card-title my-5">Card 3</h5>
            <p class="card-number">9876</p>
            <p class="card-subtitle mb-5">Subtitle 3</p>
          </div>
        </div>
      </div>
      <div class="col-md-3">
        <div class="card text-center my-last-card">
          <div class="card-body py-5">
            <h5 class="card-title my-5">Card 4</h5>
            <p class="card-number">5432</p>
            <p class="card-subtitle mb-5">Subtitle 4</p>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<style lang="scss" scoped>
.card {
  border: none;
  border-radius: 0;
  border-left: 2px solid rgb(245, 241, 237);
}

.my-last-card {
  border-right: 2px solid rgb(245, 241, 237);
}

.card-title {
  font-size: 1.5rem;
  font-weight: 900;
}

.card-number {
  font-size: 2.5rem;
  font-weight: bold;
  color: rgb(32, 173, 150);
  margin-top: 10px;
}

.card-subtitle {
  font-size: 1rem;
  font-weight: 900;
  letter-spacing: 2px;
  color: #777;
  margin-top: 10px;
}
</style>
