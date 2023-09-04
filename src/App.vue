<script>
import TheHeader from "./components/TheHeader.vue";
import TheFooter from "./components/TheFooter.vue";
import Featured from "./components/Featured.vue";
import TheHero from "./components/TheHero.vue";
import Subscribe from "./components/Subscribe.vue";
import MostView from "./components/MostView.vue";
import Numbers from "./components/Numbers.vue";
import SmartTut from "./components/SmartTut.vue";

export default {
  components: {
    TheHeader,
    TheHero,
    Featured,
    SmartTut,
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
    <Numbers />
    <MostView />
    <Subscribe />
  </main>
  <TheFooter />
</template>

<style lang="scss"></style>
