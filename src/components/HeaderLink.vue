<script>
export default {
  data() {
    return {
      link: [
        {
          name: "Home",
          src: "#",
        },
        {
          name: "About",
          src: "#",
        },
        {
          name: "Services",
          src: "#",
        },
        {
          name: "Training",
          src: "#",
        },
        {
          name: "Blogs",
          src: "#",
        },
        {
          name: "Get In Toch!",
          src: "#",
        },
      ],
    };
  },
};
</script>

<template>
  <ul>
    <li>
      <img src="/img/logo.png" alt="" />
    </li>
    <li v-for="linkItem in link" :key="linkItem.name">
      <a :href="linkItem.src"> {{ linkItem.name }} </a>
    </li>
  </ul>
</template>

<style lang="scss" scoped>
@use "./../assets/styles/partials/variables" as *;

ul {
  @include my-display-center;
  padding: 0.5rem;
}
img {
  max-width: 50%;
  margin-right: 8rem;
}
li {
  list-style: none;
  a {
    color: $color-gray;
    text-decoration: none;
    &:hover {
      color: $color-orange;
    }
  }
}
li:last-child {
  background-color: $color-orange;
  padding: 0.7rem 0.9rem;
  border-radius: 2rem;
  white-space: nowrap;
  a {
    color: white;
  }
}
</style>
