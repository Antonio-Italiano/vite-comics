<script>
export default {
    name: "AppJumbotron",
    data() {
        return {

        }
    }
};
</script>

<template>

    <section id="app-jumbotron">
        <div class="container">
            <label>CURRENT SERIES</label>
        </div>
    </section>

</template>

<style lang="scss" scoped>
#app-jumbotron {
    height: 280px;
    background-image: url(../assets/img/jumbotron.jpg);
    background-size: cover;

    .container {
        height: 100%;
        display: flex;
        align-items: flex-end;
        position: relative;
    }

    label {
        position: absolute;
        left: 0;
        bottom: -17px;
        padding: 8px 30px;
        background-color: #0282F9;
        color: #fff;
    }
}
</style>