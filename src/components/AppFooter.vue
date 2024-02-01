<script>
export default {

}
</script>

<template>
    <footer>
        <div class="image-bkg">
            <div class="space-container container">
                <div class="flex-row">
                    <div class="col">
                        <ul>
                            <li>
                                <h3>DC COMICS</h3>
                            </li>
                            <li><a href="#">Characters</a></li>
                            <li><a href="#">Comics</a></li>
                            <li><a href="#">Movies</a></li>
                            <li><a href="#">Tv</a></li>
                            <li><a href="#">Games</a></li>
                            <li><a href="#">Videos</a></li>
                            <li><a href="#">News</a></li>

                        </ul>
                        <ul>
                            <li>
                                <h3>SHOP</h3>
                            </li>
                            <li><a href="#">Shop DC</a></li>
                            <li><a href="#">Shop DC Collectibles</a></li>
                        </ul>
                    </div>
                    <ul class="col">
                        <li>
                            <h3>DC</h3>
                        </li>
                        <li><a href="#">Terms Of Use</a></li>
                        <li><a href="#">Privacy Policy (New)</a></li>
                        <li><a href="#">Ad Choices</a></li>
                        <li><a href="#">Advertising</a></li>
                        <li><a href="#">Jobs</a></li>
                        <li><a href="#">Subscriptions</a></li>
                        <li><a href="#">Talent Workshop</a></li>
                        <li><a href="#">CPSC Certificates</a></li>
                        <li><a href="#">Ratings</a></li>
                        <li><a href="#">Shop Help</a></li>
                        <li><a href="#">Contact Us</a></li>

                    </ul>
                    <ul class="col">
                        <li>
                            <h3>SITES</h3>
                        </li>
                        <li><a href="#">DC</a></li>
                        <li><a href="#">Mad Magazine</a></li>
                        <li><a href="#">DC Kids</a></li>
                        <li><a href="#">DC Universe</a></li>
                        <li><a href="#">DC Power Visa</a></li>

                    </ul>


                </div>
                <div>
                    <img class="img-dc" src="../assets/img/dc-logo-bg.png" alt="Logo Dc">
                </div>
            </div>
        </div>

    </footer>
    <footer class="lower-footer">
        <div class="container space-between">
            <div>
                <button>SIGN-UP NOW!</button>
            </div>
            <div class="social-media">
                <span>FOLLOW US</span>
                <a href="#"><img src="../assets/img/footer-facebook.png" alt="Facebook"></a>
                <a href="#"><img src="../assets/img/footer-twitter.png" alt="Twitter"></a>
                <a href="#"><img src="../assets/img/footer-youtube.png" alt="Youtube"></a>
                <a href="#"><img src="../assets/img/footer-pinterest.png" alt="Pinterest"></a>
                <a href="#"><img src="../assets/img/footer-periscope.png" alt="Periscope"> </a>

            </div>

        </div>
    </footer>
</template>

<style lang="scss" scoped>
@use '../assets/scss/_variables.scss' as variables;

.image-bkg {
    background-image: url('../assets/img/footer-bg.jpg');
    background-size: cover;
    background-position: center;
    background-repeat: no-repeat;
    height: 400px;
}

h3 {
    color: white;
    margin-bottom: 10px;
}

ul {
    margin-top: 30px;
}

.space-container {
    display: flex;
    justify-content: space-between;
}

.flex-row {
    display: flex;
    gap: 40px;
}

.col {
    display: flex;
    flex-direction: column;
}

.img-dc {
    width: 380px;
    margin-top: 10px;
}

button {
    padding: 10px;
    background-color: transparent;
    color: white;
    border: 1px solid variables.$color;
    cursor: pointer;
}

span {
    color: variables.$color;
    text-wrap: nowrap;
}

.space-between {
    display: flex;
    justify-content: space-between;
}

.lower-footer {
    height: 100px;
    background-color: rgb(48, 48, 48);
    display: flex;
    align-items: center;
}

.social-media {
    display: flex;
    gap: 10px;
    align-items: center;
}

a {
    color: gray;
}
</style>