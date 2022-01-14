<template>
  <div class="card-container">
    <img :src="thumb" :alt="title">
    <h3>{{ title }}</h3>
  </div>
</template>

<script>
export default {
    name: "ComicElement",
    props: {
        thumb: String,
        title: String,
    }
}
</script>

<style lang="scss" scoped>
    .card-container {
        
        width: calc(100% / 6 - 2rem);
        margin: 1rem;
        overflow: hidden;
        
        img {
            width: 100%;
            aspect-ratio: 1 / 1;
            object-fit: cover;
            object-position: top;
        }

        h3 {
            text-transform: uppercase;
            color: white;
            font-weight: 500;
            font-size: 0.8rem;
        }
    }
</style>