<template>
    <div class="myContainer text-black">
        <!-- Logo -->
        <div class="logo-container">
            <img src="../assets/images/dc-logo.png" alt="logoDCsmall">
        </div>

        <!-- Navbar -->
        <div class="navbar">
            <ul v-for="(item, i) in liHeader" :key="i">
                <li class="text-uppercase fw-bold">
                    <a :href="item.url">{{ item.text }}</a>
                </li>
            </ul>
        </div>
    </div>
</template>

<script>
export default {
    name: 'HeaderDC',
    data() {
        return {
            liHeader: [
                {
                    text: 'characters',
                    url: '#'
                },
                {
                    text: 'comics',
                    url: '#'
                },
                {
                    text: 'movies',
                    url: '#'
                },
                {
                    text: 'tv',
                    url: '#'
                },
                {
                    text: 'games',
                    url: '#'
                },
                {
                    text: 'collectibles',
                    url: '#'
                },
                {
                    text: 'videos',
                    url: '#'
                },
                {
                    text: 'fans',
                    url: '#'
                },
                {
                    text: 'news',
                    url: '#'
                },
                {
                    text: 'shop',
                    url: '#'
                }
            ]
        }
    }
}
</script>

<style lang="scss" scoped></style>