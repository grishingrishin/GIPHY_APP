<template>
  <div class="container">
    <ul class="gifs">
      <li class="gifs__item" v-for="gif in gifs" :key="gif.id">
        <a :href="gif.url" class="gifs__gif gif">
          <img :src="gif.images.downsized_medium.url" class="gif__img" :alt="gif.title">
        </a>
      </li>
    </ul>
  </div>
</template>

<script>
import { API_KEY } from '../utils/api_key';
const axios = require('axios').default;

export default {
  name: "Trends",
  data() {
    return {
      gifs: []
    }
  },
  mounted() {
    const url = `https://api.giphy.com/v1/gifs/trending?api_key=${API_KEY}&?q=cheeseburgers`;

    axios(url)
      .then(res => {
        const { data } = res.data;
        return this.gifs = data;
      })
      .catch(err => {
        console.log(err);
      })
  }
}
</script>