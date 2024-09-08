<template>
  <div>
    <HeroSection />
    <CardSection :cards="cardList" />
  </div>
</template>

<script>
import HeroSection from "@/components/sections/HeroSection.vue";
import CardSection from "@/components/sections/CardSection.vue";

export default {
  name: "App",
  components: {
    HeroSection,
    CardSection,
  },
  data() {
    return {
      cardList: [
        {
          id: 1,
          image: "image_400x300.png",
          text: "Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat.",
        },
        {
          id: 2,
          image: "image_400x300.png",
          text: "Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua.",
        },
        {
          id: 3,
          image: "image_400x300.png",
          text: "Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco.",
        },
      ],
    };
  },
  created() {
    console.log(this.cardList); // data内のcardListを参照
  },
};
</script>
