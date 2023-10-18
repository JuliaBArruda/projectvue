<template>
  <div id="app">
    <MainNavbar />
    <MainCarousel />
    <div class="container mt-5">
      <MainSection />
      <div class="row">
        <MainPromo
          v-for="(promo, index) in promos"
          :key="index"
          :imgSrc="promo.imgSrc"
          :title="promo.title"
          :description="promo.description"
        />
      </div>
    </div>
    <MainFooter />
  </div>
</template>

<script>
import MainNavbar from "@/components/MainNavbar.vue";
import MainCarousel from "@/components/MainCarousel.vue";
import MainSection from "@/components/MainSection.vue";
import MainPromo from "@/components/MainPromo.vue";
import MainFooter from "@/components/MainFooter.vue";

export default {
  name: "App",
  components: {
    MainNavbar,
    MainCarousel,
    MainSection,
    MainPromo,
    MainFooter,
  },
  data() {
  return {
    promos: [
      {
        imgSrc: require("@/assets/img/promo1.jpg"), 
        title: "Promoções e Lançamentos",
        description: "Na SUBWAY® sempre tem uma novidade para você. Conheça nossas promoções e lançamentos.",
      },
      {
        imgSrc: require("@/assets/img/promo2.jpg"),
        title: "Delivery",
        description: "Bateu aquela fome? Peça já pelo delivery.",
      },
  
      ],
    };
  },
};
</script>

<style>
@font-face {
  font-family: "Subway Sans Cond";
  src: url('@/fonts/SubwaySansCond-Medium.ttf')
}


body {
  font-family: "Subway Sans Cond", sans-serif;
  background-color: #F7F7F7;
}
</style>
