<template>
  <div class="h1-text">{{text}}</div>
</template>

<script>
export default {
  name: "BaseHeader",
  props: {
    text: {
      type: String,
      required: true 
    }
  }
};
</script>
