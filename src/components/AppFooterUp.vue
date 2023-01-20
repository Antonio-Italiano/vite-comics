<script>
export default {
    name: "AppFooterUp",
    data() {
        return {

        }
    }
};
</script>

<template>

    <section id="footer-up">
        <div class="row container">
            <div class="col">
                <div class="col-3">
                    <div>
                        <h3>DC COMICS</h3>
                        <ul>
                            <li><a href="#">Characters</a></li>
                            <li><a href="#">Comics</a></li>
                            <li><a href="#">Movie</a></li>
                            <li><a href="#">TV</a></li>
                            <li><a href="#">Games</a></li>
                            <li><a href="#">Videos</a></li>
                            <li><a href="#">News</a></li>
                        </ul>
                        <h3>SHOP</h3>
                        <ul>
                            <li><a href="#">Shop DC</a></li>
                            <li><a href="#">Shop DC Collectibles</a></li>
                        </ul>
                    </div>
                </div>
                <div class="col-3">
                    <h3>DC</h3>
                    <ul>
                        <li><a href="#">Terms Of use</a></li>
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
                <div class="col-3">
                    <h3>SITES</h3>
                    <ul>
                        <li><a href="#">DC</a></li>
                        <li><a href="#">MAD Magazine</a></li>
                        <li><a href="#">DC Kids</a></li>
                        <li><a href="#">DC Universe</a></li>
                        <li><a href="#">DC Power Visa</a></li>

                    </ul>
                </div>
            </div>
            <div class="col">
                <figure>
                    <img src="../assets/img/dc-logo-bg.png" alt="">
                </figure>
            </div>
        </div>

    </section>

</template>

<style lang="scss" scoped>
#footer-up {
    height: calc(50vh/3 * 2);
    background-image: url(../assets/img/footer-bg.jpg);

    .row {
        height: 100%;
        display: flex;
        padding-bottom: 15px 0;

        .col {
            width: 50%;
            height: 100%;
            display: flex;

            figure {
                height: 100%;
                width: 100%;
                display: flex;
                align-items: center;
                justify-content: center;

                img {
                    height: 140%;
                }
            }

            .col-3 {
                width: calc(100% / 3);
                height: 100%;

                h3 {
                    margin: 13px 0;
                    color: #fff;
                }

                li {
                    font-size: 13px;

                    a {
                        color: #6E837C;
                    }
                }

            }
        }
    }
}
</style>