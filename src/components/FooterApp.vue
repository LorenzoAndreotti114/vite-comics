<script>
    export default {
        data() {
            return {

                ItemsList: [
                    {
                        name: "DC COMICS",
                        list: [
                            "Characters",
                            "Comics",
                            "Movies",
                            "TV",
                            "Games",
                            "Videos",
                            "News",
                        ]
                    },
                    {
                        name: "SHOP",
                        list: [
                            "Shop DC",
                            "Shop DC Collectibles",
                        ],
                    },
                    {
                        name: "DC",
                        list: [
                            "Terms Of Use",
                            "Privacy policy (New)",
                            "Ad Choices",
                            "Advertising",
                            "Jobs",
                            "Subscriptions",
                            "Talent Workshops",
                            "CPSC Certificates",
                            "Ratings",
                            "Shop Help",
                            "Contact Us",
                        ],
                    },
                    {
                        name: "SITES",
                        list: [
                            "DC",
                            "MAD Magazine",
                            "DC Kids",
                            "DC Universe",
                            "DC Power Visa",
                        ],
                    },  
                ],
            }
        }
    }
</script>

<template>
    <div class="container">

        <!-- LEFT F -->
        <div class="left-f">

            <div class="card">

                <div class="comics">

                    <!-- DC COMICS -->
                    <h2> {{ ItemsList[0].name }} </h2>
                    <ul class="f-size" v-for="(comics, index) in ItemsList[0].list">
                        <li>
                            <a href="" class="f-gray">{{ ItemsList[0].list[index] }} </a> 
                        </li>
                    </ul>

                </div>

                <div class="shop">

                    <!-- SHOP -->
                    <h2> {{ ItemsList[1].name }} </h2>
                    <ul class="f-size f-gray" v-for="(comics, index) in ItemsList[1].list">
                        <li>
                            <a href="" class="f-gray">{{ ItemsList[1].list[index] }} </a> 
                        </li>
                    </ul>

                </div>

            </div>

            <div class="card">

                <!-- DC -->
                <h2> {{ ItemsList[2].name }} </h2>
                <ul class="f-size f-gray" v-for="(comics, index) in ItemsList[2].list">
                    <li>
                        <a href="" class="f-gray">{{ ItemsList[2].list[index] }} </a> 
                    </li>
                </ul>

            </div>

            <div class="card">

                <!-- SITES -->
                <h2> {{ ItemsList[3].name }} </h2>
                <ul class="f-size f-gray" v-for="(comics, index) in ItemsList[3].list">
                    <li>
                        <a href="" class="f-gray">{{ ItemsList[3].list[index] }} </a> 
                    </li>
                </ul>

            </div>
            
        </div>

        <!-- RIGHT F -->
        <div class="right-f">
            <img src="/src/assets/img/dc-logo-bg.png" alt="">
        </div>

    </div>
</template>

<style scoped>

    img {
        object-fit: cover;
    }

    li {
        list-style-type: none;
        padding: 1% 0;
    }

    a {
        text-decoration: none;
    }

    h2 {
        color: white;
        font-size: 1.3vw;
        padding-bottom: 5%;
    }

    .f-gray {
        color: darkgrey;
    }

    .container {
        display: flex;
        justify-content: center;
        width: 100%;
        height: 40vh;
        background: url("./src/assets/img/footer-bg.jpg");
    }

    .left-f {
        display: flex;
        justify-content: space-around;
        align-items: center;
        height: 100%;
        width: 40%;
    }

    .card {
        width: 25%;
        height: 85%;
    }

    .comics {
        height: 70%;
        width: 100%;
    }

    .shop {
        height: 30%;
        width: 100%;
    }

    .right-f {
        height: 100%;
        width: 30%;
    }

</style>