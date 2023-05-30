<script>
import AppJumbo from "./AppJumbo.vue";
import AppAboutUs from "./AppAboutUs.vue";
import AppService from "./AppService.vue";
import AppChoose from "./AppChoose.vue";
import AppReview from "./AppReview.vue";

export default {
  components: { AppJumbo, AppAboutUs, AppService, AppChoose, AppReview },
};
</script>

<template>
  <AppJumbo />
  <AppAboutUs />
  <AppService />
  <AppChoose />
  <AppReview />
</template>

<style lang="scss" scoped></style>
