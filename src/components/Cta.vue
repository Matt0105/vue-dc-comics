<template>
  <section class="buy">
    <div class="container">
        <ul>
            <li><a href="#"><img src="../assets/img/buy-comics-digital-comics.png" alt=""> Digital Comics</a></li>
            <li><a href="#"><img src="../assets/img/buy-comics-merchandise.png" alt=""> DC merchandise</a></li>
            <li><a href="#"><img src="../assets/img/buy-comics-subscriptions.png" alt=""> Subscription</a></li>
            <li><a href="#"><img src="../assets/img/buy-comics-shop-locator.png" alt=""> Comic Shop Locator</a></li>
            <li><a href="#"><img src="../assets/img/buy-dc-power-visa.svg" alt=""> DC Power Visa</a></li>
        </ul>
    </div>
          
    </section>
</template>

<script>
export default {
    name: "Cta",
}
</script>

<style lang="scss" scoped>
@import "../assets/scss/partials/_variables.scss";
    .buy {
        position: relative;
        z-index: 100;
        background-color: $DC-blue;

        ul {
            display: flex;
            justify-content: space-around;
            align-items: center;
            list-style-type: none;

            li a{
                display: flex;
                align-items: center;
                text-decoration: none;
                color: white;
                text-transform: uppercase;
                padding: 2rem 1rem;
                font-size: 0.8rem;
                
                img {
                    height: 2rem;
                    margin-right: 1rem;
                }
            }
        }
    }
</style>