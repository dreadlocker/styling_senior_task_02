<template>
  <div class="whole-screen-width absolutely-centered nav-background-color">
    <div class="nav-holder content-space-between max-width">
      <img src="@/assets/images/company logo.jpg">
      <div class="nav-dropdown">
        <span class="dropdown-language">{{language}}</span>
        <span>&#9662;</span>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "NavBar",
  props: {
    language: {
      type: String,
      required: true
    }
  }
};
</script>
