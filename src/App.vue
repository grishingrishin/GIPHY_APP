<template>
  <div id="app" class="app">
    <header class="header">
      <div class="container">
        <div class="header__inner">
          <a href="/" class="header__logo logo">
            <span
              role="img"
              style="background-image: url(../assets/images/logo.svg)"
              aria-label="Логотип приложения"
            ></span>
          </a>
          <MainNavbar />
          <button type="button" class="header__hamburger hamburger">
            <span
              role="img"
              style="background-image: url(../assets/images/menu.svg);"
              aria-label="Мобильное меню"
            ></span>
          </button>
        </div>
      </div>
    </header>
  </div>
</template>

<script>
import MainNavbar from './components/MainNavbar.vue';

export default {
  name: 'App',
  components: {
    MainNavbar
  }
}
</script>
