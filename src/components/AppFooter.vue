<script>
import AppSocial from "./AppSocial.vue";
export default { components: { AppSocial } };
</script>

<template>
  <footer>
    <div class="dog">
      <img src="/img/news.png" alt="" />
      <div class="newsletter">
        <div>Subscribe to Our Newsletter</div>
        <div class="input-group flex-nowrap">
          <input
            type="text"
            class="form-control"
            placeholder="Your Email Here"
            aria-label="Username"
            aria-describedby="addon-wrapping"
          />
          <span class="input-group-text" id="addon-wrapping">@</span>
        </div>
      </div>
    </div>
    <div class="container-list">
      <ul>
        <li>
          <h3>Get in Touch</h3>
        </li>
        <li class="question">Have a Question for us?</li>
        <li>we'll answer your problem here</li>
        <li class="social"><AppSocial /></li>
      </ul>
      <ul>
        <li>
          <h3>Support</h3>
        </li>
        <li><a href="#">Contact Us</a></li>
        <li><a href="#">Online Chat</a></li>
        <li><a href="#">Whatsapp</a></li>
        <li><a href="#">Telegram</a></li>
        <li><a href="#">Snapchat</a></li>
      </ul>
      <ul>
        <li>
          <h3>About</h3>
        </li>
        <li><a href="#">About Us</a></li>
        <li><a href="#">Blog</a></li>
        <li><a href="#">Career</a></li>
        <li><a href="#">Job</a></li>
        <li><a href="#">In press</a></li>
      </ul>
      <ul>
        <li>
          <h3>Faq</h3>
        </li>
        <li><a href="#">Account</a></li>
        <li><a href="#">Order</a></li>
        <li><a href="#">Delivery</a></li>
        <li><a href="#">Payment</a></li>
        <li><a href="#">Return</a></li>
      </ul>
      <ul>
        <li>
          <h3>Contact Me</h3>
        </li>
        <li class="icon">
          <div><i class="fa-solid fa-location-arrow"></i></div>
          4500 Mercantile plaza, suite 300, fort worth,TX,76137,USA
        </li>
        <li class="icon">
          <div><i class="fa-solid fa-phone"></i></div>
          +1(817)901 3377
        </li>
        <li class="icon">
          <div><i class="fa-solid fa-envelope"></i></div>
          info@example.com
        </li>
      </ul>
    </div>
    <div class="copyright">Copyright 2022 by AttdogMilo.com</div>
  </footer>
</template>

<style lang="scss" scoped>
@use "./../assets/styles/partials/variables" as *;
@import "bootstrap/scss/bootstrap";

footer {
  background-color: black;
  color: white;
  position: relative;
  .dog {
    position: absolute;
    top: -60px;
    left: 50%;
    right: 50%;
    transform: translateX(-50%);
    width: 650px;
    height: 150px;
    display: flex;
    flex-direction: column-reverse;
    padding-left: 2rem;
    background-color: $color-orange;
    border-radius: 10px;
    .newsletter {
      position: absolute;
      right: 10px;
      top: 40px;
      font-size: 1.2rem;
    }
    img {
      width: 250px;
    }
  }
  .input-group {
    background-color: white;
    color: $color-gray;
    margin-top: 1rem;
    width: 300px;
  }
  .input-group-text {
    background-color: $color-orange;
    color: white;
    border: 2px solid white;
  }
  .form-control {
    font-size: 0.8rem;
    color: $color-oliva;
  }
  .container-list {
    display: flex;
    justify-content: space-between;
    max-width: 1150px;
    margin: auto;
    padding-top: 8rem;
    padding-bottom: 2rem;
    li {
      list-style: none;
      padding-bottom: 0.7rem;
      a {
        text-decoration: none;
        color: white;
      }
    }
    h3 {
      padding-bottom: 1.7rem;
      color: $color-orange;
    }
  }
}
.question {
  margin-bottom: -0.7rem;
}
.social {
  padding-top: 1rem;
}
.icon {
  display: flex;
  i {
    padding-right: 0.7rem;
    color: $color-orange;
  }
}
.container-list ul:first-child,
.container-list ul:last-child {
  width: 25%;
}
.copyright {
  display: flex;
  justify-content: center;
  border-top: 1px solid #232323;
  padding: 2rem 0 1rem;
}
</style>
