<script>
export default {
    name: "AppMainDown",
    data() {
        return {
            data: [
                {
                    image: 'buy-comics-digital-comics.png',
                    alt: 'Digital Comics'
                },
                {
                    image: 'buy-comics-merchandise.png',
                    alt: 'Dc Merchandise'
                },
                {
                    image: 'buy-comics-subscriptions.png',
                    alt: 'Subscription'
                },
                {
                    image: 'buy-comics-shop-locator.png',
                    alt: 'Comic Shop Locator'
                },
                {
                    image: 'buy-dc-power-visa.svg',
                    alt: 'Dc Power Visa'
                },
            ]

        }
    },
    methods: {
        buildImagePath(image) {
            const url = new URL(`../assets/img/${image}`, import.meta.url);
            return url.href
        }
    }
};
</script>

<template>

    <section id="main-down">
        <div class="row container">
            <div class="col-5" v-for="(d, i) in data">
                <figure>
                    <a href="#">
                        <img :src="buildImagePath(d.image)" alt="d.alt">
                        <p>{{ d.alt.toUpperCase() }}</p>
                    </a>
                </figure>
            </div>
        </div>
    </section>

</template>

<style lang="scss" scoped>
#main-down {
    height: calc(100vh/6 + 40px);
    background-color: #0282F9;

    .row {
        display: flex;
        height: 100%;

        .col-5 {
            width: calc(100%/5);
            height: 100%;

            figure {
                height: 100%;
                width: 100%;
                display: flex;
                justify-content: center;
                align-items: center;

                a {
                    height: 30%;
                    width: 80%;
                    display: flex;
                    align-items: center;

                    img {
                        max-height: 100%;
                    }

                    p {
                        color: #fff;
                        margin-left: 10px;
                        font-size: 12px;
                    }
                }
            }
        }
    }
}
</style>