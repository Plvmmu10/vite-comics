<template>
    <div class="myContainer">
        <ul>
            <li class="d-flex align-items-center px-3" v-for="(item, i) in liMain" :key="i">
                <div class="icons-box">
                    <img :src="'/images/' + item.image">
                </div>

                <p class="icons-text text-uppercase">
                    {{ item.text }}
                </p>

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
    width: 40px;
    margin: 0 .5rem;

    img {
        width: 100%;
    }
}

.icons-text {
    font-size: 20px;
    margin: 0;
}
</style>