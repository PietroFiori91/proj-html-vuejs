<script>
import TheHeader from "./components/TheHeader.vue";
import TheFooter from "./components/TheFooter.vue";
import Featured from "./components/Featured.vue";
import TheHero from "./components/TheHero.vue";
import Subscribe from "./components/Subscribe.vue";
import MostView from "./components/MostView.vue";
import Numbers from "./components/Numbers.vue";

export default {
  components: {
    TheHeader,
    TheHero,
    Featured,
    Numbers,
    MostView,
    Subscribe,
    TheFooter,
  },
};
</script>

<template>
  <TheHeader />
  <TheHero />
  <main>
    <Featured />
    <Numbers />
    <MostView />
    <Subscribe />
  </main>
  <TheFooter />
</template>

<style lang="scss"></style>
