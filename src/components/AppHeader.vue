<script>
import HeaderLink from "./HeaderLink.vue";
import AppSocial from "./AppSocial.vue";

export default { components: { HeaderLink, AppSocial } };
</script>

<template>
  <div class="top-bar">
    <div class="content-top-bar">
      <div class="contacts">
        <span><i class="fa-solid fa-envelope"></i>info@example.com</span>
        <span><i class="fa-solid fa-phone"></i>+1(817)901 3377</span>
      </div>
      <AppSocial />
    </div>
  </div>
  <HeaderLink />
</template>

<style lang="scss" scoped>
@use "./../assets/styles/partials/variables" as *;
.top-bar {
  background-color: $color-oliva;
  .content-top-bar {
    @include my-display-center;
    height: 3.5rem;
  }
}
.contacts {
  color: white;
  i {
    padding-inline: 0.6rem;
    color: $color-orange;
  }
}
</style>
