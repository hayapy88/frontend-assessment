<template>
  <div class="items">
    <h1 class="items__title">Items list</h1>
    <div class="items__list">
      <Item
        v-for="(item, index) in items"
        :key="index"
        :title="item.title"
        :content="item.content"
        :icon="item.icon"
        :isActive="index === activeIndex"
        @toggle="toggleItem(index)"
      />
    </div>
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
  data() {
    return {
      activeIndex: 0,
    };
  },
  methods: {
    toggleItem(index) {
      console.log("Toggling item at index:", index);
      this.activeIndex = this.activeIndex === index ? -1 : index;
    },
  },
};
</script>
