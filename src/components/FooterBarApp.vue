<script>
    export default {
        data() {
            return {
                icons: [
                    {
                        name: "facebook",
                        src: "./src/assets/img/footer-facebook.png"
                    },
                    {
                        name: "twitter",
                        src: "./src/assets/img/footer-twitter.png"
                    },
                    {
                        name: "youtube",
                        src: "./src/assets/img/footer-youtube.png"
                    },
                    {
                        name: "pinterest",
                        src: "./src/assets/img/footer-pinterest.png"
                    },
                    {
                        name: "periscope",
                        src: "./src/assets/img/footer-periscope.png"
                    },
                ],
            }
        }
    }
</script>

<template>
    <div class="container">

        <!-- LEFT BTN -->
        <div class="left">
            <button>SIGN-UP NOW!</button>
        </div>

        <!-- RIGHT ICONS UL -->
        <div class="right">

            <!-- TITLE -->
            <div class="follow">
                <h2>FOLLOW US</h2>
            </div>

            <div class="inner-icons">
                <ul class="f-size">
                    <li v-for="(iconsInput, index) in icons">
                        <a href=""><img :src="icons[index].src" :alt="icons[index].name"></a>
                    </li>
                </ul>
            </div>
        </div>

    </div>
</template>

<style scoped>

    button {
        color: white;
        font-size: 1vw;
        background-color: rgb(51, 51, 51);
        border: 2px solid rgb(0, 102, 255);
        padding: 2%;
    }

    img {
        object-fit: contain;
    }

    h2 {
        color: rgb(0, 102, 255);
    }

    li {
        list-style-type: none;
        height: 100%;
        padding: 3%;
    }

    ul {
        display: flex;
        justify-content: center;
        align-items: center;
        padding: 8%;
    }

    .container {
        display: flex;
        justify-content: center;
        width: 100%;
        height: 14vh;
        background-color: rgb(51, 51, 51);
    }

    .left {
        display: flex;
        justify-content: baseline;
        align-items: center;
        height: 100%;
        width: 35%;
    }
    
    .right {
        display: flex;
        height: 100%;
        width: 35%;
    }

    .follow {
        display: flex;
        justify-content: end;
        align-items: center;
        height: 100%;
        width: 40%;
    }

    .inner-icons {
        display: flex;
        height: 100%;
        width: 60%;
    }

</style>