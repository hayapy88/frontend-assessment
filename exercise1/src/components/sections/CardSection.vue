<template>
  <div class="card-section">
    <Card
      v-for="card in cards"
      :key="card.id"
      :image="card.image"
      :text="card.text"
    />
  </div>
</template>

<script>
import Card from "@/components/ui/Card.vue";
export default {
  name: "CardSection",
  components: {
    Card,
  },
  props: {
    cards: {
      type: Array,
      Required: true,
    },
  },
};
</script>
