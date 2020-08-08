<template>
  <section class="section">
    <div class="container">
      <div class="section__header">
        <h2 class="section__title">
          {{ title }}
        </h2>
        <a :href="link" class="section__detail">See all</a>
      </div>
      <slot></slot>
    </div>
  </section>
</template>

<script>
export default {
  name: 'Section',
  props: {
    title: {
      type: String,
    },
    link: {
      type: String
    }
  }
}
</script>