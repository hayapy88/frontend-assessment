<template>
  <div class="item">
    <p class="item__title">{{ title }}</p>
    <div class="item__content" v-html="content"></div>
  </div>
</template>

<script>
export default {
  name: "Item",
  props: {
    title: { type: String, required: true },
    content: { type: String, required: true },
  },
};
</script>
