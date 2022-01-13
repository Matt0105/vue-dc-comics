<template>
  <div class="main-content">
      <h1>--Content goes here--</h1>
      <section class="buy">
          <ul>
              <li><a href="#"><img src="../assets/img/buy-comics-digital-comics.png" alt=""> Digital Comics</a></li>
              <li><a href="#"><img src="../assets/img/buy-comics-merchandise.png" alt=""> DC merchandise</a></li>
              <li><a href="#"><img src="../assets/img/buy-comics-subscriptions.png" alt=""> Subscription</a></li>
              <li><a href="#"><img src="../assets/img/buy-comics-shop-locator.png" alt=""> Comic Shop Locator</a></li>
              <li><a href="#"><img src="../assets/img/buy-dc-power-visa.svg" alt=""> DC Power Visa</a></li>
          </ul>
      </section>
  </div>
</template>

<script>
export default {
    name: "Main",
}
</script>

<style lang="scss" scoped>
@import "../assets/scss/partials/_variables.scss";

    .main-content {
        
        width: 100%;
        background-color: black;
    }
    
    h1 {
        color: white;
    }

    .buy {
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