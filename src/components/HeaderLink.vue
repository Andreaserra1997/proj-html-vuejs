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
ul {
  display: flex;
  justify-content: space-between;
  align-items: center;
  max-width: 1150px;
  margin: auto;
  background-color: #f5f5f5;
  padding: 0.5rem;
}
img {
  max-width: 50%;
  margin-right: 8rem;
}
li {
  list-style: none;
  a {
    color: #444444;
    text-decoration: none;
    &:hover {
      color: #ce7c2a;
    }
  }
}
li:last-child {
  background-color: #ce7c2a;
  padding: 0.7rem 0.9rem;
  border-radius: 2rem;
  white-space: nowrap;
  a {
    color: white;
  }
}
</style>
