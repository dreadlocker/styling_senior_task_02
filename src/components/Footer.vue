<template>
  <div class="footer flex content-space-between">
    <FooterFirstColumn />
    <FooterNexttColumn
      v-for="(text, index) in headerTextArray"
      :key="index"
      :headerText="text"
      :arrayWithObjects="text2dArray[index]"
    />
    <FooterLastColumn
      :headerText="socialHeaderText"
      :imagesSrcArray="socialImagesSrcArray"
    />
  </div>
</template>

<script>
import FooterFirstColumn from "./FooterFirstColumn.vue";
import FooterNexttColumn from "./FooterNexttColumn.vue";
import FooterLastColumn from "./FooterLastColumn.vue";

export default {
  name: "Footer",
  components: {
    FooterFirstColumn,
    FooterNexttColumn,
    FooterLastColumn
  },
  props: {
    headerTextArray: {
      type: Array,
      required: true
    },
    text2dArray: {
      type: Array,
      required: true
    },
    socialHeaderText: {
      type: String,
      required: true
    },
    socialImagesSrcArray: {
      type: Array,
      required: true
    }
  }
};
</script>
