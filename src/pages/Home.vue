<template>
  <div class="homepage">
    <section class="section trending">
      <div class="container">
        <div class="section__header trending__header">
          <h2 class="section__title trending__title">
            Trending GIFs
          </h2>
          <a href="/" class="section__all trending__all">See All</a>
        </div>
        <Trends/>
      </div>
    </section>
    <section class="section artists">
      <div class="container">
        <div class="section__header artists__header">
          <h2 class="section__title artists__title">
            Artists
          </h2>
          <a href="/" class="section__all trending__all">See All Artists</a>
        </div>
        <Artists/>
      </div>
    </section>
    <section class="section stroies">
      <div class="container">
        <div class="section__header stroies__header">
          <h2 class="section__title stroies__title">
            All Stories
          </h2>
        </div>
        <Stories/>
      </div>
    </section>
  </div>
</template>

<script>
import Trends from "../components/Trends.vue";
import Artists from "../components/Artists.vue";
import Stories from "../components/Stories.vue";

export default {
  name: "Home",
  components: {
    Trends,
    Artists,
    Stories,
  }
}
</script>