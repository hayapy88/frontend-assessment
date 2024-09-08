<template>
  <div class="card">
    <div class="card__content">
      <div class="card__image">
        <img :src="imageSrc" alt="Card image" />
      </div>
      <p class="card__text">
        {{ text }}
      </p>
    </div>
    <div class="card__button">
      <Button></Button>
    </div>
  </div>
</template>

<script>
import Button from "./Button.vue";
import image400x300 from "@/assets/images/image_400x300.png";

export default {
  name: "Card",
  components: {
    Button,
  },
  props: {
    image: {
      type: String,
      required: true,
    },
    text: {
      type: String,
      required: true,
    },
  },
  computed: {
    imageSrc() {
      return image400x300;
    },
  },
};
</script>
