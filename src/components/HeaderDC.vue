<template>
    <div class="myContainer text-black align-items-center">
        <!-- Logo -->
        <div class="logo-container">
            <img src="/images/dc-logo.png" alt="logoDCsmall">
        </div>

        <!-- Navbar -->
        <div class="navbar">
            <ul>
                <li class="text-uppercase fw-bold d-none d-xxl-flex" v-for="(item, i) in liHeader" :key="i">
                    <a :href="item.url" :class="i === currentIndex ? 'active' : ''" @click="getActive(i)">{{ item.text
                    }}</a>
                </li>

                <i class="fa-solid fa-bars d-flex d-xxl-none"></i>

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
            ],
            currentIndex: 0
        }
    },
    methods: {
        getActive(index) {
            this.currentIndex = index;
        }
    }
}
</script>

<style lang="scss" scoped>
.myContainer {
    height: 100%;
    padding: 0;

    .navbar {
        height: 100%;
        padding: 0;

        ul {
            height: 100%;
            padding: 0;
            display: flex;
            align-items: center;
            justify-content: center;
            flex-wrap: wrap;

            li {
                height: 100%;
                padding: 0;
                margin: 0 .7rem;
                display: flex;
                justify-content: center;
                align-items: center;



                a {
                    height: 100%;
                    display: flex;
                    align-items: center;

                    &:hover {
                        border-bottom: 5px solid #0282f9;
                    }
                }
            }

            i {
                display: flex;
                font-size: 40px;
            }
        }
    }
}
</style>