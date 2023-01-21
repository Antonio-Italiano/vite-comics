<script>
export default {
    name: "AppFooterDown",
    data() {
        return {

        }
    }
};
</script>

<template>

    <section id="footer-down">
        <div class="row container">
            <div class="col">
                <button>
                    <a href="#">SIGN-UP NOW!</a>
                </button>
            </div>
            <div class="col">
                <div class="center">
                    <a href="#">FOLLOW US</a>
                    <figure>
                        <a href="#"><img src="../assets/img/footer-facebook.png" alt="social"></a>
                        <a href="#"><img src="../assets/img/footer-periscope.png" alt="social"></a>
                        <a href="#"><img src="../assets/img/footer-pinterest.png" alt="social"></a>
                        <a href="#"><img src="../assets/img/footer-twitter.png" alt="social"></a>
                        <a href="#"><img src="../assets/img/footer-youtube.png" alt="social"></a>
                    </figure>
                </div>
            </div>
        </div>

    </section>

</template>

<style lang="scss" scoped>
#footer-down {
    height: calc(50vh/3 - 40px);
    background-color: #303030;
    position: relative;

    .row {
        height: 100%;
        display: flex;

        .col {
            width: 50%;
            display: flex;
            align-items: center;

            .center {
                height: 100%;
                width: 100%;
                display: flex;
                justify-content: center;
                align-items: center;

                a {
                    margin-right: 10px;
                }
            }


            img {
                padding: 0 10px;
                height: 60%;
            }

            a {
                color: #0282F9;
            }

            button {
                background-color: transparent;
                border: 0;

                a {
                    color: #fff;
                    padding: 10px;
                    border: 2px solid #0282F9;
                }
            }
        }
    }
}
</style>