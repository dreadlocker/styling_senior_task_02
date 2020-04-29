<template>
  <div class="footer-last-column">
    <div class="footer-h1-text">{{headerText}}</div>
    <div class="flex content-space-between footer-links-holder">
      <div
        v-for="(src, index) in imagesSrcArray"
        :key="index"
        class="footer-social-img-holder"
      ><img :src="src" class="footer-social-img"></div>
    </div>
  </div>
</template>

<script>
export default {
  name: "FooterLastColumn",
  props: {
    headerText: {
      type: String,
      required: true
    },
    imagesSrcArray: {
      type: Array,
      required: true
    }
  },
};
</script>
