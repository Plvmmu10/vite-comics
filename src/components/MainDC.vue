<template>
    <div class="myContainer text-white flex-wrap">
        <CardDC :thumb="item.thumb" :series="item.series" v-for="item in comicsList" />
    </div>
</template>

<script>
import CardDC from './CardDC.vue';
import { comics } from '../assets/data/data.js';
export default {
    name: "MainDC",
    components: {
        CardDC
    },
    data() {
        return {
            comicsList: [...comics]
        }
    }
}
</script>

<style lang="scss" scoped>
.myContainer {
    padding: 2rem 0;
}
</style>