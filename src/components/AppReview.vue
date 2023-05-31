<script>
export default {
  data() {
    return {
      arrReview: [
        {
          title: "Great Place",
          description:
            "Lorem Ipsum is simply dummy text of the printing and typesetting industry. Lorem Ipsum has been the industry's standard dummy text ever since the 1500s, when",
          img: "/img/t1.png",
          author: "Tobias May",
          job: "UI/UX Designer",
        },
        {
          title: "Great Place",
          description:
            "Lorem Ipsum is simply dummy text of the printing and typesetting industry. Lorem Ipsum has been the industry's standard dummy text ever since the 1500s, when",
          img: "/img/t1.png",
          author: "Tobias May",
          job: "UI/UX Designer",
        },
      ],
    };
  },
};
</script>

<template>
  <div class="icon">
    <img src="/img/dog-icon.png" />
    <span>Review & Rating</span>
  </div>
  <div class="container-review">
    <div class="rating">
      <div class="title">Over 8000 Customers With 5-Star Review</div>
      <div class="description">
        It is a long established fact that a reader will be distructed by the
        readable content of a page when looking at its layout.
      </div>
      <div>
        <i
          v-for="i in 5"
          :key="i"
          class="fa-sharp fa-solid fa-star"
          style="color: #eeff00"
        ></i>
      </div>
    </div>
    <div v-for="review in arrReview" :key="review" class="review">
      <div class="star">
        <i
          v-for="i in 5"
          :key="i"
          class="fa-sharp fa-solid fa-star"
          style="color: #eeff00"
        ></i>
      </div>
      <div class="title-review">{{ review.title }}</div>
      <div class="description-review">{{ review.description }}</div>
      <div class="author">
        <img :src="review.img" />
        <div class="text-author">
          <div class="name">{{ review.author }}</div>
          <div class="job">{{ review.job }}</div>
        </div>
      </div>
    </div>
  </div>
  <div class="arrow">
    <img src="/img/left-arrow.png" alt="" />
    <img src="/img/next.png" alt="" />
  </div>
</template>

<style lang="scss" scoped>
@use "./../assets/styles/partials/variables" as *;

.icon {
  display: flex;
  align-items: center;
  max-width: 1150px;
  margin: auto;
  padding-top: 4rem;
  img {
    width: 20px;
  }
  span {
    color: $color-oliva;
    font-size: 0.7rem;
    padding-left: 0.7rem;
  }
}
.container-review {
  display: flex;
  max-width: 1150px;
  margin: auto;
  padding-top: 2rem;
  gap: 4rem;
}
.rating {
  width: calc((100% / 3) - 2rem);
  .title {
    width: 80%;
    font-size: 1.7rem;
    padding-bottom: 2rem;
  }
  .description {
    padding-bottom: 2rem;
    line-height: 1.3rem;
  }
}
.review {
  width: calc((100% / 3) - 2rem);
  padding: 1rem;
  background-color: $color-light-white;
  .star {
    padding-bottom: 1rem;
  }
  .title-review {
    font-size: 1.3rem;
    padding-bottom: 1.3rem;
  }
  .description-review {
    line-height: 1.3rem;
    padding-bottom: 1.3rem;
  }
  .author {
    display: flex;
    align-items: center;
    img {
      width: 60px;
      border-radius: 50%;
    }
    .text-author {
      padding-left: 0.5rem;
      .name {
        font-size: 1.2rem;
        padding-bottom: 0.8rem;
      }
    }
  }
}
.arrow {
  display: flex;
  justify-content: end;
  max-width: 1150px;
  margin: auto;
  gap: 1rem;
  padding-top: 1rem;
  padding-bottom: 10rem;
  img {
    width: 40px;
    background-color: $color-orange;
    padding: 0.5rem;
  }
}
</style>
