<template>
  <nav class="navbar">
    <ul class="navbar__nav nav">
      <li class="nav__item" v-for="(route, index) in routes" :key="index">
        <a :href="route.url" class="nav__link">{{ route.name }}</a>
      </li>
    </ul>
  </nav>
</template>

<script>
export default {
  name: "MainNavbar",
  data() {
    return {
      routes: [
        {
          name: 'Reactions',
          url: '/reactions/'
        },
        {
          name: 'Entertainment',
          url: '/entertainment'
        },
        {
          name: 'Sports',
          url: '/sports/'
        },
        {
          name: 'Stickers',
          url: '/stickers/'
        },
        {
          name: 'Artists',
          url: '/artists'
        },
      ]
    }
  }
}
</script>