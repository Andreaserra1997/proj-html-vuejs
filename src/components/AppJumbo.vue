<script>
export default {};
</script>

<template>
  <div class="jumbo">
    <div class="content-jumbo">
      <div class="title">Welcome to <span>DogMilo</span> Pets</div>
      <p>
        Lorem Ipsum is simply dummy text of the printing and typesetting
        industry.
      </p>
      <div class="content-btn">
        <span class="btn">Get Started</span>
        <img src="/img/play.png" class="video" />
      </div>
    </div>
  </div>
</template>

<style lang="scss" scoped>
@use "./../assets/styles/partials/variables" as *;

.jumbo {
  height: 573px;
  background-image: url(../../public/img/b.png);
  background-size: cover;
  background-repeat: no-repeat;
  background-position: center;
}
.content-jumbo {
  max-width: 1150px;
  margin: auto;
  padding-top: 13rem;
  color: white;
}
.title {
  font-size: 2rem;
  font-weight: bold;
  width: 250px;
  line-height: 3rem;
  span {
    font-weight: 400;
  }
}
p {
  width: 330px;
  padding: 1.3rem 0 1.3rem;
}
.content-btn {
  display: flex;
  align-items: center;
}
.btn {
  background-color: $color-orange;
  padding: 0.7rem 1rem;
  border-radius: 2rem;
  white-space: nowrap;
}
.video {
  width: 40px;
  background-color: #71d0f6;
  margin-left: 0.5rem;
  padding: 0.5rem;
  border-radius: 0.5rem;
}
</style>
