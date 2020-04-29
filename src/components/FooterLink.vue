<template>
  <a :href="linkHref" class="footer-link" >{{linkText}}<br></a>
</template>

<script>
export default {
  name: "FooterLink",
  props: {
    linkHref: {
      type: String,
      required: true 
    },
    linkText: {
      type: String,
      required: true 
    }
  }
};
</script>
