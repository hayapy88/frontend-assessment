<template>
  <div class="item" :class="{ 'is-active': isActive }">
    <h2 class="item__header" @click="$emit('toggle')">
      <component :is="getIcon" class="item__icon size-5 text-black" />
      {{ title }}
      <component
        :is="isActive ? ChevronUpIcon : ChevronDownIcon"
        class="item__chevron size-4"
      />
    </h2>
    <div class="item__content" v-if="isActive" v-html="content"></div>
  </div>
</template>

<script>
import * as SolidIcons from "@heroicons/vue/24/solid";

export default {
  name: "Item",
  props: {
    title: { type: String, required: true },
    content: { type: String, required: true },
    icon: { type: String, required: true },
    isActive: { type: Boolean, default: false },
  },
  computed: {
    getIcon() {
      return SolidIcons[this.icon];
    },
    ChevronUpIcon() {
      return SolidIcons.ChevronUpIcon;
    },
    ChevronDownIcon() {
      return SolidIcons.ChevronDownIcon;
    },
  },
};
</script>
