<template>
  <div class="footer-next-column">
    <div class="footer-h1-text">{{headerText}}</div>
    <div class="footer-links-holder">
      <FooterLink
        v-for="(obj, index) in arrayWithObjects"
        :key="index"
        :linkHref="obj.href"
        :linkText="obj.linkText"
      />
    </div>
  </div>
</template>

<script>
import FooterLink from "./FooterLink.vue";

export default {
  name: "FooterNexttColumn",
  components: {
    FooterLink
  },
  props: {
    headerText: {
      type: String,
      required: true
    },
    arrayWithObjects: {
      type: Array,
      required: true
    },
  },
};
</script>
