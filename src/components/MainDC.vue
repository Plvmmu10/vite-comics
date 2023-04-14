<template>
    <div class="myContainer text-white flex-wrap">
        <span class="text-uppercase fw-bold">current series</span>
        <CardDC :thumb="item.thumb" :series="item.series" v-for="item in comicsList" />
        <div class="btn-container d-flex justify-content-center align-items-center w-100">
            <button class="btn btn-primary text-uppercase rounded-0 fw-bold">load more</button>
        </div>

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
    position: relative;

    span {
        position: absolute;
        top: -20px;
        padding: .7rem 1.5rem;
        background-color: #0282f9;
    }
}
</style>