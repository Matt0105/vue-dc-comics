<template>
    <div class="header-container">
        <div class="container">
            <img src="../assets/img/dc-logo.png" alt="">
            <ul>
                <li><a href="#">Characters</a></li>
                <li><a href="#" class="active">Comics</a></li>
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
        width: 100%;
        height: 80px;
        background-color: white;
    }

    .container {
        display: flex;
        justify-content: space-between;
        align-items: center;
        width: 80%;
        height: 100%;
        margin: 0 auto;
    }

    img {
        height: 80%;
    }

    ul {
        display: flex;
        list-style-type: none;

        li a{
            margin: 0 0.8rem;
            padding: calc(80px / 2 - 0.8rem + 2px) 0; //altezza header / 2 - altezza font + (bordo / 2)
            text-decoration: none;
            color: black;
            text-transform: uppercase;
            font-size: 0.8rem;
            font-weight: 600;

            &:hover,
            &:active,
            &.active {
                color: $DC-blue;
                border-bottom: 4px solid $DC-blue;
            }
        }
    }

    .jumbo img {
        height: 500px;
    }
</style>