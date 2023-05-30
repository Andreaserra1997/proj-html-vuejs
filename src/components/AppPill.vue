<script>
export default {
  data() {
    return {
      arrPill: [
        {
          img: "/img/d-1.png",
          title: "Pet Sitting",
          text: "The readable content of a page when looking at its layout.",
        },
        {
          img: "/img/d-2.png",
          title: "Puppy Sitting",
          text: "The readable content of a page when looking at its layout.",
        },
        {
          img: "/img/d-3.png",
          title: "Dog Walking",
          text: "The readable content of a page when looking at its layout.",
        },
        {
          img: "/img/d-4.png",
          title: "Night Care",
          text: "The readable content of a page when looking at its layout.",
        },
        {
          img: "/img/d-5.png",
          title: "Pet Sitting",
          text: "The readable content of a page when looking at its layout.",
        },
      ],
    };
  },
};
</script>

<template>
  <div class="content-pill">
    <div v-for="pill in arrPill" :key="pill.img" class="pill">
      <img :src="pill.img" class="pill-img" />
      <h3>{{ pill.title }}</h3>
      <p>{{ pill.text }}</p>
      <img src="/img/right.png" class="icon-img" />
    </div>
  </div>
</template>

<style lang="scss" scoped>
@use "./../assets/styles/partials/variables" as *;

.content-pill {
  display: flex;
  max-width: 1150px;
  margin: auto;
  gap: 3rem;
  padding-inline: 1rem;
  color: white;
  .pill {
    background-color: $color-orange;
    border-radius: 3rem;
    text-align: center;
    height: 300px;
    border-radius: 50% / 60px;
    .pill-img {
      width: 35%;
      padding: 1rem 0 1.5rem;
    }
    h3 {
      padding-bottom: 1rem;
    }
    p {
      padding-bottom: 1.5rem;
    }
    .icon-img {
      background-color: $color-yellow;
      width: 60px;
      height: 60px;
      border-radius: 50%;
      padding: 1.2rem;
    }
  }
}
</style>
