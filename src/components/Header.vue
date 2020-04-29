<template>
  <div class="flex content-space-between header-holder">
    <div class="flex">
      <div
        v-for="(src, index) in imagesSrcArray"
        :key="index"
        class="flex"
      >
        <img :src="src" class="header-icon">
        <span class="header-text">{{textArray[index]}}</span>
      </div>
    </div>

    <div>
      <BaseButton
        v-for="(text, index) in buttonTextArray"
        :key="index"
        :text="buttonTextArray[index]"
        :class="[
          index < buttonTextArray.length - 1 ? 'btn-normal' : 'btn-success',
          {'btn-margin-left': index > 0}
        ]"
      />
    </div>
  </div>
</template>

<script>
import BaseButton from "./BaseButton.vue";

export default {
  name: "Header",
  components: {
    BaseButton,
  },
  props: {
    imagesSrcArray: {
      type: Array,
      required: true 
    },
    textArray: {
      type: Array,
      required: true 
    },
    buttonTextArray: {
      type: Array,
      required: true 
    },
  },
};
</script>
