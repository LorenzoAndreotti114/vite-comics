<script>
    export default {
        data() {
            return {
                icons: [
                    {
                        name: "DIGITAL COMICS",
                        src: "./src/assets/img/buy-comics-digital-comics.png"
                    },
                    {
                        name: "DC MERCANDISE",
                        src: "./src/assets/img/buy-comics-merchandise.png"
                    },
                    {
                        name: "SUBSCRIPTION",
                        src: "./src/assets/img/buy-comics-subscriptions.png"
                    },
                    {
                        name: "COMIC SHOP LOCATOR",
                        src: "./src/assets/img/buy-comics-shop-locator.png"
                    },
                    {
                        name: "DC POWER VISA",
                        src: "./src/assets/img/buy-dc-power-visa.svg"
                    },
                ]
            }
        }
    }
</script>

<template>
    <div class="container">
        <div class="card f-size" v-for="(iconsCards, index) in icons">

            <div class="icon-card">
                <img :src=" icons[index].src " alt="">
            </div>

            <a href="">{{ icons[index].name }}</a>

        </div>
    </div>
</template>

<style scoped>

    img {
        object-fit: contain;
    }

    a {
        text-decoration: none;
        color: white;
    }

    .container {
        display: flex;
        justify-content: center;
        background-color: rgb(0, 102, 255);
        width: 100%;
        height: 20vh;
    }

    .card {
        display: flex;
        align-items: center;
        height: 100%;
        width: 15%;
        color: white;
    }

    .icon-card {
        height: 30%;
        width: 20%;
        margin-right: 3%;
    }

</style>