<template>
  <Items :items="itemList" />
</template>

<script>
import Items from "@/components/Items.vue";
import itemList from "@/data/data.json";
export default {
  name: "App",
  components: {
    Items,
  },
  data() {
    return {
      itemList,
    };
  },
};
</script>
