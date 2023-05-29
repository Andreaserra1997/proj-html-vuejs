<script>
import HeaderLink from "./HeaderLink.vue";

export default { components: { HeaderLink } };
</script>

<template>
  <div class="top-bar">
    <div class="content-top-bar">
      <div class="contacts">
        <span><i class="fa-solid fa-envelope"></i>info@example.com</span>
        <span><i class="fa-solid fa-phone"></i>+1(817)901 3377</span>
      </div>
      <div class="social">
        <img src="../../public/img/icon_Facebook.png" />
        <img src="../../public/img/icon_Pinterest.png" />
        <img src="../../public/img/icon_Twitter.png" />
        <img src="../../public/img/icon_Linkedin.png" />
        <img src="../../public/img/icon_Instagram.png" />
      </div>
    </div>
  </div>
  <HeaderLink />
</template>

<style lang="scss" scoped>
.top-bar {
  background-color: #7f7045;
  .content-top-bar {
    display: flex;
    justify-content: space-between;
    align-items: center;
    max-width: 1150px;
    height: 3.5rem;
    margin: auto;
  }
}
.contacts {
  color: white;
  i {
    padding-inline: 0.6rem;
    color: #ce7c2a;
  }
}
.social {
  img {
    width: 30px;
    padding-inline: 0.2rem;
  }
}
</style>
