<template>
    <div class="header-container">
        <img src="../assets/img/dc-logo.png" alt="">
        <ul>
            <li><a href="#">Characters</a></li>
            <li><a href="#">Comics</a></li>
            <li><a href="#">Movies</a></li>
            <li><a href="#">Tv</a></li>
            <li><a href="#">Games</a></li>
            <li><a href="#">Collectables</a></li>
            <li><a href="#">Videos</a></li>
            <li><a href="#">Fans</a></li>
            <li><a href="#">News</a></li>
            <li><a href="#">Shop</a></li>
        </ul>
    </div>
</template>

<script>
export default {
    name: "Header",
    data() {
        return {

        }
    }
}
</script>

<style lang="scss" scoped>
@import "../assets/scss/partials/_variables.scss";

    .header-container {
        display: flex;
        justify-content: space-between;
        align-items: center;
        width: 100%;
        height: 80px;
        background-color: white;
    }

    img {
        height: 80%;
    }

    ul {
        display: flex;
        list-style-type: none;

        li a{
            padding: 1rem 0;
            margin: 0 1rem;
            text-decoration: none;
            color: black;
            text-transform: uppercase;
            font-size: 0.8rem;
            font-weight: 600;

            &:hover {
                color: $DC-blue;
                border-bottom: 4px solid $DC-blue;
            }
        }
    }
</style>