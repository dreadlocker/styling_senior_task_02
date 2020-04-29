<template>
  <div>
    <div class="sports-categories-icon-text-wrapper max-width">
      <div
        v-for="(src, index) in iconsSrcArray"
        :key="index"
        class="sports-categories-icon-text-holder"
      >
        <div class="sports-categories-icon-holder absolutely-centered">
          <img :src="src" class="sports-categories-icon">
        </div>
        <span class="sports-categories-icon-text">{{iconsTextArray[index]}}</span>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "SportsCategories",
  props: {
    iconsSrcArray: {
      type: Array,
      required: true
    },
    iconsTextArray: {
      type: Array,
      required: true
    },
  },
};
</script>
