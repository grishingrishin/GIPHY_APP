<template>
  <form class="search-form">
    <div class="container">
      <div class="search-form__main">
        <input
          type="text"
          class="search-form__input"
          autocapitalize="off"
          autocorrect="off"
          autocomplete="off"
          placeholder="Search all the GIFs and Stickers"
        >
        <button type="submit" class="search-form__submit" aria-label="Кнопка поиска">
          <span
            role="img"
            style="background-image: url(images/search.svg);"
            aria-label="Иконка лупы"
          ></span>
        </button>
      </div>
    </div>
  </form>
</template>

<script>
export default {
  name: "SearchInput"
}
</script>