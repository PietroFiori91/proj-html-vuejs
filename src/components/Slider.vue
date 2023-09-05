<script>
export default {
  props: {
    slides: Array,
  },
  data() {
    return {
      currentIndex: 0,
    };
  },
  methods: {
    setCurrentSlide(index) {
      this.currentIndex = index;
    },
  },
};
</script>

<template>
  <div class="my-container py-5">
    <div class="slider-container">
      <div class="slider d-flex justify-content-center gap-4">
        <div
          v-for="(slide, index) in slides"
          :key="index"
          class="slide"
          :style="{ opacity: currentIndex === index ? 1 : 0.5 }"
        >
          <div class="slide-content">
            <p class="slide-title">{{ slide.title }}</p>
            <p class="slide-description">{{ slide.description }}</p>
            <div class="user-profile d-flex align-items-center">
              <img
                :src="slide.profileImg"
                alt="Profile Image"
                class="profile-img"
              />
              <div class="user-info d-flex flex-column">
                <p class="user-name">{{ slide.userName }}</p>
                <p class="user-role">{{ slide.userRole }}</p>
              </div>
            </div>
          </div>
        </div>
      </div>
      <div class="slider-dots d-flex justify-content-center mt-5">
        <span
          v-for="(slide, index) in slides"
          :key="index"
          class="slider-dot"
          :class="{ active: currentIndex === index }"
          @click="setCurrentSlide(index)"
        ></span>
      </div>
    </div>
  </div>
</template>

<style lang="scss" scoped>
.my-container {
  background-color: rgb(248, 248, 248);
}
.slider-container {
  width: 100%;
  max-width: 450px;
  margin: 0 auto;
}

.slider {
  transition: transform 0.5s ease-in-out;
}

.slide {
  flex: 0 0 100%;
}

.slide-content {
  padding: 20px;
  background-color: white;
}

.profile-img {
  width: 40px;
  height: 40px;
  border-radius: 50%;
  margin-right: 10px;
}

.slider-dot {
  width: 12px;
  height: 12px;
  background-color: #b8b8b8;
  border-radius: 50%;
  margin: 0 6px;
  cursor: pointer;
  transition: background-color 0.5s ease-in-out;
}
</style>
