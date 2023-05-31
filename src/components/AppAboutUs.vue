<script>
export default {};
</script>

<template>
  <div class="background-img">
    <div class="container">
      <div class="square-left">
        <img src="/img/about.png" />
      </div>
      <div class="square-right">
        <div class="about">
          <div class="icon">
            <img src="/img/dog-icon.png" />
            <span>About us</span>
          </div>
          <div class="title">Welcome DogMilo Pets</div>
          <p>
            Lorem Ipsum is simply dummy text of the printing and typesetting
            industry. Lorem Ipsum has been the insudtry's standard dummy text
            ever since the 1500s, when an unknown printer took a galley of type
            and scrambled
          </p>
          <p>
            Lorem Ipsum is simply dummy text of the printing and typesetting
            industry. Lorem Ipsum has been the insudtry's standard dummy text
            ever since the 1500s, when an unknown printer took a galley of type
            and scrambled
          </p>
        </div>
      </div>
    </div>
  </div>
</template>

<style lang="scss" scoped>
@use "./../assets/styles/partials/variables" as *;

.background-img {
  background-image: url(./../../public/img/dog-logo.png);
  background-repeat: no-repeat;
  background-position-x: right;
  background-position-y: 20%;
  background-size: 12%;
}
.container {
  display: flex;
  max-width: 1150px;
  margin: auto;
}
.square-left {
  width: 50%;
  padding: 4rem 2rem 4rem 0;
  img {
    width: 80%;
  }
}
.square-right {
  width: 50%;
  display: flex;
  align-items: center;
}
.about {
  .icon {
    display: flex;
    align-items: center;
    span {
      color: $color-oliva;
      font-size: 0.7rem;
      padding-left: 0.7rem;
    }
  }
  .title {
    padding-top: 2rem;
    font-size: 2rem;
  }
  p {
    padding-top: 2rem;
  }
}
</style>
