<template>
    <div class="col-12 col-md-4 col-lg-2 p-3">
        <div class="card bg-transparent border-0">

            <div class="card-body">
                <!-- Card image -->
                <div class="card-img">
                    <img :src="thumb" :alt="series" class="img-fluid">
                </div>
                <!-- Card title -->
                <div class="card-title py-2">
                    <h6 class="text-uppercase">{{ series }}</h6>
                </div>
            </div>
        </div>
    </div>
</template>

<script>
export default {
    props: ['thumb', 'series'],
    name: 'CardDC'
}
</script>

<style lang="scss" scoped>
.card-img {
    width: 100%;
    height: 200px;

    img {
        width: 100%;
        height: 100%;
    }
}
</style>