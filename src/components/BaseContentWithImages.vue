<template>
  <div class="flex content-space-between">
    <img
      v-for="(src, _) in imagesSrcArray"
      :key="_"
      :src="src"
      class="top-content-img"
    >
  </div>
</template>

<script>
export default {
  name: "BaseContentWithImages",
  props: {
    imagesSrcArray: {
      type: Array,
      required: true
    }
  }
};
</script>
