<script>
import AppJumbo from "./AppJumbo.vue";
import AppAboutUs from "./AppAboutUs.vue";
import AppService from "./AppService.vue";
import AppChoose from "./AppChoose.vue";

export default {
  components: { AppJumbo, AppAboutUs, AppService, AppChoose },
};
</script>

<template>
  <AppJumbo />
  <AppAboutUs />
  <AppService />
  <AppChoose />
</template>

<style lang="scss" scoped></style>
