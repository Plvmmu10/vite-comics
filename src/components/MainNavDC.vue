<template>
    <div class="myContainer">
        <ul>
            <li class="d-flex align-items-center px-3" v-for="(item, i) in liMain" :key="i">
                <div class="icons-box">
                    <img :src="'/images/' + item.image">
                </div>

                <a href="#">
                    <p class="icons-text text-uppercase">
                        {{ item.text }}
                    </p>
                </a>


            </li>
        </ul>
    </div>
</template>

<script>
export default {
    name: 'MainNavDC',
    data() {
        return {
            liMain: [
                {
                    image: 'buy-comics-digital-comics.png',
                    text: 'digital comics'
                },
                {
                    image: 'buy-comics-merchandise.png',
                    text: 'dc merchandise'
                },
                {
                    image: 'buy-comics-subscriptions.png',
                    text: 'subscriptions'
                },
                {
                    image: 'buy-comics-shop-locator.png',
                    text: 'comic shop locator'
                },
                {
                    image: 'buy-dc-power-visa.svg',
                    text: 'dc power visa'
                }
            ]
        }
    }
}
</script>

<style lang="scss" scoped>
.icons-box {
    width: 50px;
    height: 50px;
    margin: 0 .5rem;

    img {
        width: 100%;
        height: 100%;
        object-fit: contain;
        object-position: center;
    }
}

.icons-text {
    font-size: 17px;
    margin: 0;
}

.myContainer {
    justify-content: center;

    ul {
        padding: 0;
        display: flex;
        flex-wrap: wrap;

        li {
            cursor: pointer;

            a {
                color: white;
            }
        }

    }
}
</style>