<script>
    export default {
        data() {
            return {
                menu: [
                    {
                        name: "CHARACTERS",
                    },
                    {
                        name: "COMICS",
                    },
                    {
                        name: "MOVIES",
                    },
                    {
                        name: "TV",
                    },
                    {
                        name: "GAMES",
                    },
                    {
                        name: "COLLECTIBLES",
                    },
                    {
                        name: "VIDEOS",
                    },
                    {
                        name: "FANS",
                    },
                    {
                        name: "NEWS",
                    },
                    {
                        name: "SHOP",
                    },
                ]
            }
        }
    }

</script>

<template>
    <div class="container">

        <!-- LEFT H -->
        <div class="left-h">
            <img src="../assets/img/dc-logo.png" alt="">
        </div>

        <!-- RIGHT H -->
        <div class="right-h">
            <ul>
                <li class="f-size" v-for="(menuList, index) in menu"><a href="">{{ menu[index].name }}</a></li>
            </ul>
        </div>
    </div>
</template>

<style scoped>

img {
    object-fit: contain;
    padding: 2%;
}

ul {
    height: 100%;
}

li {
    display: flex;
    align-items: center;
    height: 100%;
    list-style-type: none;

    &:hover {
        border-bottom: 6px solid blue;

        a {
            color: blue;
        }

    }
}

a {
    text-decoration: none;
    color: black;
    font-weight: 600;
}

.container {
    width: 100%;
    display: flex;
    /* DEBUG */
    height: 120px;
    background-color: aqua;
}

.left-h {
    width: 30%;
    height: 100%;
}

.right-h {
    width: 70%;
    height: 100%;
    display: flex;
    justify-content: center;
    align-items: center;
    ul {
        display: flex;
        justify-content: center;
        align-items: center;

        li {
            padding: 0% 2%;
        }
    }
}

</style>