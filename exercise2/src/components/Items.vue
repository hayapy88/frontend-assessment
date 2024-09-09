<template>
  <div class="items">
    <Item
      v-for="(item, index) in items"
      :key="index"
      :title="item.title"
      :content="item.content"
    />
  </div>
</template>

<script>
import Item from "@/components/Item.vue";
export default {
  name: "Items",
  components: {
    Item,
  },
  props: { items: { type: Array, required: true } },
};
</script>
