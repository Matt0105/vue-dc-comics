<template>
  <div class="card-container">
    <div class="thumb">

        <div class="type-label">
            <span>{{ type }}</span>
        </div>
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
        price: String,
        type: String
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

            &:hover img {
                opacity: 0.3;
            }

            &:hover .price-label {
                opacity: 1;
            }

            &:hover .type-label {
                opacity: 0.8;
                top: 0;
            }

            .price-label, .type-label {
                position: absolute;
                left: 50%;
                z-index: 100;
                background-color: $DC-blue;
                color: white;
                opacity: 0;
                transition: all 0.4s;
            }

            .price-label{
                top: 50%;
                transform: translate(-50%, -50%);
                padding: 0.6rem 1rem;
                border-radius: 5px;
                cursor: pointer;
            }

            .type-label {
                top: -30px;
                display: flex;
                justify-content: center;
                align-items: center;
                @include dimensions(80%, 30px);
                transform: translateX(-50%);
                text-transform: uppercase;
                font-size: 0.8rem;
            }

        }
 
    }
</style>