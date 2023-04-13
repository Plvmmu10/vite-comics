<template>
    <div class="myContainer text-black">
        <!-- Logo -->
        <div class="logo-container">
            <img src="/images/dc-logo.png" alt="logoDCsmall">
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
                    url: '#',
                    active: false
                },
                {
                    text: 'comics',
                    url: '#',
                    active: false
                },
                {
                    text: 'movies',
                    url: '#',
                    active: false
                },
                {
                    text: 'tv',
                    url: '#',
                    active: false
                },
                {
                    text: 'games',
                    url: '#',
                    active: false
                },
                {
                    text: 'collectibles',
                    url: '#',
                    active: false
                },
                {
                    text: 'videos',
                    url: '#',
                    active: false
                },
                {
                    text: 'fans',
                    url: '#',
                    active: false
                },
                {
                    text: 'news',
                    url: '#',
                    active: false
                },
                {
                    text: 'shop',
                    url: '#',
                    active: false
                }
            ]
        }
    }
}
</script>

<style lang="scss" scoped></style>