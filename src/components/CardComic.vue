<template>
  <div class="card-comic">
      <img :src="comicThumb" :alt="cardSeries">
      <h2>{{ comicSeries }}</h2>
  </div>
</template>

<script>
export default {
    name: 'CardComic',
    props: {
        comicThumb: String,
        comicSeries: String
    }
}
</script>

<style>

</style>