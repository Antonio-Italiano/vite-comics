<script>
export default {
    name: "AppMainUp",
    data() {
        return {

        }
    }
};
</script>

<template>

    <section id="main-up">
        <div class="container">
            <h2>--> Content goes here --> </h2>
        </div>
    </section>

</template>

<style lang="scss" scoped>
#main-up {
    height: calc(100vh/6);
    background-color: black;

    .container {
        height: 100%;
        color: #fff;
        display: flex;
        align-items: center;
    }
}
</style>