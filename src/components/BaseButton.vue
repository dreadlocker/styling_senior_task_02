<template>
  <button class="btn">{{text}}</button>
</template>

<script>
export default {
  name: "BaseButton",
  props: {
    text: {
      type: String,
      required: true 
    },
  },
};
</script>
