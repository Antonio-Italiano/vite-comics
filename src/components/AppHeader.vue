<script>
export default {
    name: "AppHeader",
    data() {
        return {

            currentIndex: 1,
            data: [
                {
                    text: 'Characters',
                    url: '#',
                    current: false,
                },
                {
                    text: 'Comics',
                    url: '#',
                    current: true,
                },
                {
                    text: 'Movies',
                    url: '#',
                    current: false,
                },
                {
                    text: 'TV',
                    url: '#',
                    current: false,
                },
                {
                    text: 'Games',
                    url: '#',
                    current: false,
                },
                {
                    text: 'Collectibles',
                    url: '#',
                    current: false,
                },
                {
                    text: 'Videos',
                    url: '#',
                    current: false,
                },
                {
                    text: 'Fans',
                    url: '#',
                    current: false,
                },
                {
                    text: 'News',
                    url: '#',
                    current: false,
                },
                {
                    text: 'Shop',
                    url: '#',
                    current: false,
                },
            ]
        }
    },
    methods: {
        setCurrentIndex(index) {
            this.currentIndex = index;
        }
    }
};
</script>

<template>
    <header>
        <div class="row container">
            <div class="col-40">
                <a href="#">
                    <img src="../assets/img/dc-logo.png" alt="logo-dc">
                </a>
            </div>
            <div class="col-60">
                <nav>
                    <ul>
                        <li v-for="(d, i) in data" :key="d.text">
                            <a :href="d.url" :class="{ 'cliched': currentIndex === i }" @click="setCurrentIndex(i)">{{
                                d.text.toUpperCase()
                            }}</a>
                        </li>
                    </ul>
                </nav>
            </div>
        </div>
    </header>
</template>

<style lang="scss" scoped>
header {
    height: calc(100vh/6);

    .row {
        height: 100%;
        display: flex;

        .col-40 {
            width: 40%;
            padding: 10px 0;

            a {
                display: flex;
                align-items: center;
                height: 100%;
                width: 21%;

                img {
                    height: 70%;
                }
            }
        }

        .col-60 {
            width: 60%;

            nav {
                height: 100%;

                ul {
                    display: flex;
                    align-items: center;
                    height: 100%;

                    li {
                        padding: 0 10px;
                        height: 100%;
                        display: flex;
                        align-items: center;
                    }

                    a {
                        font-size: 12px;
                        color: black;
                        height: 100%;
                        display: flex;
                        align-items: center;
                        border-bottom: 5px solid transparent;

                        &.cliched,
                        &:hover {
                            border-bottom: 5px solid #1596FA;
                            color: #1596FA;
                        }
                    }
                }
            }
        }
    }
}
</style>