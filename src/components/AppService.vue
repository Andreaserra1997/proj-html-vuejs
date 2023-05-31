<script>
import AppPill from "./AppPill.vue";
export default { components: { AppPill } };
</script>

<template>
  <div class="background-img">
    <div class="content">
      <div class="title">Service</div>
      <div class="description">
        DogMilo Pet Care Services For Your Best Friends.
      </div>
      <AppPill />
    </div>
    <img src="../../public/img/dog-left.png" class="img-dog" />
  </div>
</template>

<style lang="scss" scoped>
@use "./../assets/styles/partials/variables" as *;

.background-img {
  background-color: $color-light-white;
  background-image: url(./../../public/img/dog-logo.png);
  background-repeat: no-repeat;
  background-position-x: right;
  background-position-y: 20%;
  background-size: 12%;
  position: relative;
  padding-bottom: 3rem;
}
.img-dog {
  position: absolute;
  top: 100px;
  width: 10%;
}
.content {
  text-align: center;
  .title {
    color: $color-oliva;
  }
}
.content:first-child {
  padding-top: 3rem;
}
.description {
  padding: 1.5rem 0 2.5rem;
  font-size: 2rem;
  width: 400px;
  margin: auto;
}
</style>
