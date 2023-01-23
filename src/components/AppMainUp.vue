<script>
export default {
    name: "AppMainUp",
    props: {
        cards: Array
    },
    data() {
        return {

        }
    }
};
</script>

<template>

    <section id="main-up">
        <div class="row container">
            <!-- CREATED CARD  -->
            <div v-for="c in cards" class="col-card" :key="c.series">
                <figure>
                    <a href="#">
                        <img :src="c.thumb" :alt="c.series">
                        <h5>{{ c.series }}</h5>
                    </a>
                </figure>
            </div>
            <div class="col">
                <button><a href="#">LOAD MORE</a></button>
            </div>
        </div>
    </section>

</template>

<style lang="scss" scoped>
#main-up {
    min-height: calc(100vh/6);
    background-color: #1C1C1C;

    .row {
        display: flex;
        flex-wrap: wrap;
        align-items: center;
        height: 520px;
        padding: 30px 0;

        .col-card {
            height: 150px;
            width: calc(100%/6);
            margin-bottom: 60px;
        }

    }

    figure {
        height: 100%;
        width: 100%;
        padding: 0 20px;

        a {
            display: block;
            height: 100%;
            color: #fff;
        }

        img {
            height: 100%;
            width: 100%;
        }
    }

    .col {
        width: 100%;
        margin-top: 20px;
        display: flex;
        justify-content: center;

        button {
            border: 0;

            a {
                padding: 8px 30px;
                background-color: #0282F9;
                color: #fff;

            }
        }
    }


}
</style>