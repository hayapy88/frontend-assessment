<template>
  <div>
    <img :src="imageSrc" alt="Card image" />
    <p>{{ text }}</p>
  </div>
  <Button>Button</Button>
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
