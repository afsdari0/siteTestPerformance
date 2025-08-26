<template>
  <div class="d-flex justify-center ga-6 mt-4">
    <a
      v-for="(item, i) in socialLinks"
      :key="i"
      :href="item.url"
      target="_blank"
      rel="noopener noreferrer"
      class="social-link"
    >
      <svg-icon type="mdi" :path="item.icon" class="icon" />
    </a>
  </div>
</template>

<script>
import SvgIcon from "@jamescoyle/vue-icon";
import { mdiInstagram, mdiFacebook, mdiLinkedin, mdiTwitter } from "@mdi/js";

export default {
  name: "SocialIcons",
  components: { SvgIcon },
  data() {
    return {
      socialLinks: [
        { name: "Instagram", icon: mdiInstagram, url: "https://instagram.com" },
        { name: "Facebook", icon: mdiFacebook, url: "https://facebook.com" },
        { name: "LinkedIn", icon: mdiLinkedin, url: "https://linkedin.com/company" },
        { name: "X", icon: mdiTwitter, url: "https://x.com" }
      ]
    };
  }
};
</script>

<style scoped>
.social-link {
  display: flex;
  align-items: center;
  justify-content: center;
  transition: opacity 0.3s ease;
}
.social-link:hover {
  opacity: 0.6; /* perde opacidade no hover */
}
.icon {
  width: 32px;
  height: 32px;
  opacity: 1 !important;
  color: white;
}
</style>