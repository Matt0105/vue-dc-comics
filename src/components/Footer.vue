<template>
  <div class="footer-container">
      <div class="container">

        <div class="col">
        <h2>Dc Comics</h2>
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

        <h2>Shop</h2>
        <ul>
            <li><a href="#">Shop DC</a></li>
            <li><a href="#">Shop DC Collections</a></li>
            
        </ul>
        </div>

        <div class="col">
            <h2>DC</h2>
            <ul>
                <li><a href="#">Terms Of Use</a></li>
                <li><a href="#">Privacy policy (New)</a></li>
                <li><a href="#">Ad Choices</a></li>
                <li><a href="#">Advertising</a></li>
                <li><a href="#">Jobs</a></li>
                <li><a href="#">Subscriptions</a></li>
                <li><a href="#">Talent Workshops</a></li>
                <li><a href="#">CPSC Certificates</a></li>
                <li><a href="#">Ratings</a></li>
                <li><a href="#">Shop Help</a></li>
                <li><a href="#">Contact Us</a></li>
            </ul>
        </div>

        <div class="col">
            <h2>Sites</h2>
            <ul>
                <li><a href="#">DC</a></li>
                <li><a href="#">MAD Magazine</a></li>
                <li><a href="#">DC Kids</a></li>
                <li><a href="#">DC Universe</a></li>
                <li><a href="#">DC Power Visa</a></li>
            </ul>
        </div>

        <div class="col-img">
            <img src="../assets/img/dc-logo-bg.png" alt="">
        </div>
        
      </div>

    <div class="footer-bottom">
        <div class="container">
            <button>Sign Up Now!</button>

            <div class="social">
                <h2>Follow us</h2>
                <ul>
                    <li><a href="#"><img src="../assets/img/footer-facebook.png" alt=""></a></li>
                    <li><a href="#"><img src="../assets/img/footer-twitter.png" alt=""></a></li>
                    <li><a href="#"><img src="../assets/img/footer-youtube.png" alt=""></a></li>
                    <li><a href="#"><img src="../assets/img/footer-pinterest.png" alt=""></a></li>
                    <li><a href="#"><img src="../assets/img/footer-periscope.png" alt=""></a></li>
                </ul>
            </div>
        </div>
        
    </div>

  </div>
</template>

<script>
export default {
    name: "Footer",
}
</script>

<style lang="scss" scoped>
@import "../assets/scss/partials/_variables.scss";
    .footer-container {
        width: 100%;
        background-image: url(../assets/img/footer-bg.jpg);
        
    }
    .container {
        display: flex;
        // background-image: url(../assets/img/dc-logo-bg.png);
        // background-repeat: no-repeat;
        // background-position:right;
        // background-size: contain;
    }

    .col {
        h2 {
            margin-top: 2rem;
            margin-bottom: 0.8rem;
            margin-right: 2rem;
            text-transform: uppercase;
            color: white;
        }

        ul {
            list-style-type: none;
            margin-bottom: 2rem;

            li a {
                display: block;
                text-decoration: none;
                color: gray;
                padding: 0.3rem;
                padding-right: 0.5rem;
        }
        }
    }

    .footer-bottom {
        display: flex;
        align-items: center;
        width: 100%;
        height: 80px;
        background-color: $footer-color;
    }

    .footer-bottom > .container {
        justify-content: space-between;
    }

    button {
            border: 1px solid $DC-blue;
            background-color: $footer-color;
            padding: 1rem;
            text-transform: uppercase;
            color: white;
        }

    .social {
        display: flex;
        align-items: center;
        h2 {
            font-size: 1.3rem;
            color: $DC-blue;
            text-transform: uppercase;
        }
        ul {
            display: flex;
            list-style-type: none;
            margin-left: 1rem;

            li {
                margin-right: 0.7rem;
            }
        }
    }
    


</style>