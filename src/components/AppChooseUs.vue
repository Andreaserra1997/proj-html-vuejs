<script>
export default {
  data() {
    return {
      arrChoose: [
        {
          img: "/img/w-3.png",
          title: "Safety First",
          text: "It is a long established fact that a reader will be distructed by the readable content of a page when looking at its layout.",
        },
        {
          img: "/img/w-2.png",
          title: "Play Yards",
          text: "It is a long established fact that a reader will be distructed by the readable content of a page when looking at its layout.",
        },
        {
          img: "/img/w-1.png",
          title: "Monitor Your Pets",
          text: "It is a long established fact that a reader will be distructed by the readable content of a page when looking at its layout.",
        },
      ],
    };
  },
};
</script>

<template>
  <div v-for="choose in arrChoose" :key="choose.img" class="chooses">
    <img :src="choose.img" />
    <div class="text">
      <div class="title">{{ choose.title }}</div>
      <p>{{ choose.text }}</p>
    </div>
  </div>
</template>

<style lang="scss" scoped>
.chooses {
  display: flex;
  img {
    width: 18%;
  }
  .text {
    display: flex;
    flex-direction: column;
    padding-left: 1rem;
    p {
      line-height: 1.4rem;
    }
  }
  .title {
    padding-bottom: 1.5rem;
    font-size: 1.3rem;
  }
}
.chooses:nth-child(even) {
  justify-content: end;
  .text {
    width: 65%;
  }
}
.chooses:last-child {
  justify-content: end;
  .text {
    width: 45%;
  }
}
</style>
