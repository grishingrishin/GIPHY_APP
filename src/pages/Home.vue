<template>
  <div class="homepage">
    <PageSection title="Trending GIFs">
      <AllTrands/>
    </PageSection>
    <PageSection title="Artists">
      <Artists/>
    </PageSection>
    <PageSection title="All Stories">
      <Stories/>
    </PageSection>
  </div>
</template>

<script>
import PageSection from "../components/PageSection.vue";
import AllTrands from "../sections/AllTrands.vue";
import Artists from "../sections/Artists.vue";
import Stories from "../sections/Stories.vue";

export default {
  name: "Home",
  components: {
    PageSection,
    AllTrands,
    Artists,
    Stories,
  }
}
</script>