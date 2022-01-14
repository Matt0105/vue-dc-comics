<template>
  <div class="card-container">
    <div class="thumb">
        <img :src="thumb" :alt="title">
        <div class="price-label">
            <span>{{ price }}</span>
        </div>
    </div>
    <h3>{{ title }}</h3>
  </div>
</template>

<script>
export default {
    name: "ComicElement",
    props: {
        thumb: String,
        title: String,
        price: String
    }
}
</script>

<style lang="scss" scoped>
 @import "../assets/scss/partials/_variables.scss";
 @import "../assets/scss/partials/_mixins.scss";

    .card-container {
        @include dimensions(calc(100% / 6 - 2rem), none);
        margin: 1rem;
        overflow: hidden;
        
        img {
            @include dimensions(100%, none);
            aspect-ratio: 1 / 1;
            object-fit: cover;
            object-position: top;
            transition: all 0.3s;

        }

        h3 {
            text-transform: uppercase;
            color: white;
            font-weight: 500;
            font-size: 0.8rem;
        }

        .thumb {
            position: relative;
            background-color: black;
            transition: all 0.3s;

            &:hover {
                opacity: 1;
            }

            &:hover img{
                opacity: 0.3;
            }

            &:hover .price-label{
                opacity: 0.8;
            }

        }

        .price-label {
            position: absolute;
            top: 50%;
            left: 50%;
            transform: translate(-50%, -50%);
            z-index: 100;
            padding: 0.8rem 1.2rem;
            background-color: $DC-blue;
            color: white;
            border-radius: 5px;
            opacity: 0;
            transition: all 0.3s;
            cursor: pointer;
        }
    }
</style>