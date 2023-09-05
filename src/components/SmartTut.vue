<script>
export default {
  // PASSING DATA FROM PARENT TO CHILD COMPONENT=PROPS
  props: {
    subtitle: String,
    title: String,
    cards: Array,
    videoUrl: String,
    infoSubtitle: String,
    infoTitle: String,
    infoParagraph: String,
  },
};
</script>

<template>
  <div class="my-container">
    <div class="container">
      <div class="my-container py-5">
        <!-- CENTER TITLES -->
        <h2 class="text-center pb-1">{{ subtitle }}</h2>
        <h1 class="text-center pb-5">{{ title }}</h1>

        <!-- CARDS X3 -->
        <div class="row justify-content-center">
          <div v-for="(card, index) in cards" :key="index" class="col-md-4">
            <div class="card">
              <img
                src="../assets/img/about-us-02-image-box-02.png"
                class="card-img-top"
                alt="Card Image"
              />
              <div class="card-body">
                <h5 class="card-title">{{ card.title }}</h5>
                <p class="card-text">{{ card.description }}</p>
                <button class="btn">
                  <span class="my-btn">Learn More</span>
                </button>
              </div>
            </div>
          </div>
        </div>
      </div>

      <!-- BOTTOM CONTAINER -->
      <div class="row justify-content-center my-4 py-5">
        <!-- VIDEO PANEL -->
        <!-- non vedo cover img -->
        <div class="col-md-6">
          <iframe
            width="670"
            height="450"
            :src="videoUrl"
            frameborder="0"
            poster="../assets/img/home-2-popup-video-poster.jpg"
          ></iframe>
        </div>

        <!-- INFO PANEL DX -->
        <div class="col-md-4 offset-md-1">
          <h3>{{ infoSubtitle }}</h3>
          <h2>{{ infoTitle }}</h2>
          <p>{{ infoParagraph }}</p>
          <button class="btn">{{ infoButton }}</button>
        </div>
      </div>
    </div>
  </div>
</template>

<style lang="scss" scoped>
.my-container {
  border-bottom-left-radius: 50%;
}
.container {
  padding: 5rem 0;
}
.my-btn {
  font-size: 0.8rem;
  font-weight: 700;
}

img {
  width: 250px;
  height: auto;
}

.card {
  border: none;
}
</style>
