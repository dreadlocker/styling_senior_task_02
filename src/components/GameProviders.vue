<template>
  <div class="flex content-space-between game-providers-content-holder">
    <div
      v-for="(src, index) in imageSrcArray"
      :key="index"
      class="game-providers-image-holder"
    >
      <img :src="src" class="game-providers-image">
    </div>
  </div>
</template>

<script>
export default {
  name: "GameProviders",
  props: {
    imageSrcArray: {
      type: Array,
      required: true
    },
  },
};
</script>
