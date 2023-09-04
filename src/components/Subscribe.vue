<!-- IMPORTA VARIABILI DI SASS -->

<script>
export default {
  data() {
    return {
      // STORING USER EMAIL
      email: "",
    };
  },
  methods: {
    // TRIGGER TO USER SUBMITS
    subscribe() {
      //LOGGING MSG WITH USER EMAIL
      console.log("Subscribed with email:", this.email);
      // CLEAR INPUT
      this.email = "";
    },
  },
};
</script>

<template>
  <div class="container py-5">
    <div class="row justify-content-center">
      <div class="col-md-6">
        <div class="vertical-column text-center p-4">
          <h1 class="title">Subscribe <span>Newsletter</span></h1>
          <p class="paragraph">
            Subscribe to receive the latest updates and news.
          </p>
          <form class="subscribe-form" @submit.prevent="subscribe">
            <div class="form-group input-group">
              <input
                v-model="email"
                type="email"
                class="form-control"
                placeholder="Enter your email"
                required
              />
              <div class="input-group-append">
                <button type="submit" class="btn subscribe-btn">
                  Subscribe
                </button>
              </div>
            </div>
          </form>
        </div>
      </div>
    </div>
  </div>
</template>

<style lang="scss" scoped>
.subscribe-btn {
  position: absolute;
  bottom: 10px;
  right: 0;
  margin: 0;
  padding: 6px 20px;
}

span {
  color: rgb(32, 173, 150);
  font-weight: 400;
}
.vertical-column {
  background-color: #ffffff;
  border-radius: 10px;
}

.title {
  font-size: 24px;
  font-weight: bold;
  margin-bottom: 20px;
  color: rgb(63, 58, 100);
}

.paragraph {
  font-size: 18px;
  margin-bottom: 20px;
}

.subscribe-form {
  display: flex;
  flex-direction: column;
  align-items: center;
}

.form-control {
  background-color: rgb(245, 245, 245);
  width: 100%;
  padding: 10px;
  margin-bottom: 10px;
  border: none;
  border-radius: 5px;
}

.btn {
  background-color: rgb(32, 173, 150);
  color: #fff;
  border: none;
  padding: 10px 20px;
  border-radius: 5px;
  cursor: pointer;
}
</style>
