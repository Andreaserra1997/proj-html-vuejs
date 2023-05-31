<script>
import AppChooseUs from "./AppChooseUs.vue";

export default { components: { AppChooseUs } };
</script>

<template>
  <div class="container">
    <div class="square-img">
      <img src="/img/why.png" alt="" />
    </div>
    <div class="square-text">
      <div class="icon">
        <img src="/img/dog-icon.png" />
        <span>Choose us</span>
      </div>
      <div class="title">Why Choose Us?</div>
      <AppChooseUs />
    </div>
  </div>
</template>

<style lang="scss" scoped>
@use "./../assets/styles/partials/variables" as *;

.container {
  display: flex;
  gap: 3rem;
}
.square-img {
  width: 50%;
  img {
    width: 100%;
  }
}
.square-text {
  width: 50%;
  .icon {
    display: flex;
    align-items: center;
    padding-top: 3rem;
    img {
      width: 50px;
    }
    span {
      color: $color-oliva;
      font-size: 0.7rem;
      padding-left: 0.7rem;
    }
  }
}
.title {
  font-size: 2rem;
  padding: 1.5rem 0 2rem;
}
</style>
