<script>
    import CardBanner from './CardBanner.vue';

    export default {

        components: {
            CardBanner,
        },

        data() {
            return {

            }
        }
    }
</script>

<template>
    <div class="container">

        <div class="top-banner">
            <img src="/src/assets/img/jumbotron.jpg" alt="">
        </div>


        <CardBanner />

    </div>
</template>

<style scoped>

    img {
        object-fit: cover;
        object-position: 0 0;
    }

    .container {
        width: 100%;
        height: 120vh;
        background-color: rgb(37, 37, 37);
    }

    .top-banner {
        height: 30%;
        width: 100%;
    }

</style>