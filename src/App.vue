<script>
import TheHeader from "./components/TheHeader.vue";
import TheFooter from "./components/TheFooter.vue";
import Featured from "./components/Featured.vue";
import TheHero from "./components/TheHero.vue";
import Subscribe from "./components/Subscribe.vue";
import MostView from "./components/MostView.vue";
import Numbers from "./components/Numbers.vue";
import SmartTut from "./components/SmartTut.vue";
import Slider from "./components/Slider.vue";

export default {
  components: {
    TheHeader,
    TheHero,
    Featured,
    SmartTut,
    Slider,
    Numbers,
    MostView,
    Subscribe,
    TheFooter,
  },
  data() {
    return {
      cardData: [
        {
          title: "Card 1 Title",
          description: "Card 1 Description",
        },
        {
          title: "Card 1 Title",
          description: "Card 1 Description",
        },
        {
          title: "Card 1 Title",
          description: "Card 1 Description",
        },
      ],
      sliderData: [
        {
          title: "High level of efficiency and scientific methods",
          description: "Description 1",
          profileImg: "profile1.jpg",
          userName: "User 1",
          userRole: "Role 1",
        },
        {
          title: "Slide 2",
          description: "Description 2",
          profileImg: "profile2.jpg",
          userName: "User 2",
          userRole: "Role 2",
        },
        {
          title: "High level of efficiency and scientific methods",
          description: "Description 3",
          profileImg: "profile3.jpg",
          userName: "User 3",
          userRole: "Role 3",
        },
      ],
    };
  },
};
</script>

<template>
  <TheHeader />
  <TheHero />
  <main>
    <Featured />
    <div>
      <SmartTut
        :subtitle="'Centered Subtitle'"
        :title="'Centered Title'"
        :cards="cardData"
        :videoUrl="'https://www.youtube.com/embed/VIDEO_ID'"
        :infoSubtitle="'Info Subtitle'"
        :infoTitle="'Info Title'"
        :infoParagraph="'Info Paragraph Text'"
        :infoButton="'Info Button'"
      />
    </div>
    <div>
      <Slider :slides="sliderData" />
    </div>
    <Numbers />
    <MostView />
    <Subscribe />
  </main>
  <TheFooter />
</template>

<style lang="scss"></style>
