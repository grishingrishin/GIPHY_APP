<template>
  <div id="app">
    <header class="header">
      <div class="container">
        <div class="header__inner">
          <a href="/" class="header__logo logo">
            <span
              role="img"
              style="background-image: url(images/logo.svg)"
              aria-label="Логотип приложения"
            ></span>
          </a>
          <MainNavbar />
          <button type="button" class="header__hamburger hamburger">
            <span
              role="img"
              style="background-image: url(images/menu.svg);"
              aria-label="Мобильное меню"
            ></span>
          </button>
        </div>
      </div>
    </header>
    <SearchInput />
    <div class="content-area">
      <main class="main">
        <Home />
      </main>
    </div>
  </div>
</template>

<script>
// Components
import MainNavbar from './components/MainNavbar.vue';
import SearchInput from "./components/SearchInput.vue";

// Pages
import Home from './pages/Home.vue';

export default {
  name: 'App',
  components: {
    MainNavbar,
    SearchInput,
    Home
  }
}
</script>
