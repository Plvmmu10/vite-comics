<template>
    <div id="hero">
        <img src="/images/jumbotron.jpg" alt="jumbo">
    </div>
</template>

<script>
export default {
    name: 'JumbotronDC'
}
</script>

<style lang="scss" scoped>
#hero {
    height: 350px;

    img {
        max-height: 100%;
        width: 100%;
        object-fit: cover;
        object-position: top;
    }
}
</style>