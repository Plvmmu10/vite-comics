<template>
    <div class="top-footer">
        <div class="listContainer">
            <ul v-for="(item, index) in footerLi" :key="index">
                <h1>{{ item[obj].title }}</h1>

                <ul>

                </ul>
            </ul>
        </div>

        <div class="img-box">

        </div>
    </div>

    <div class="bottom-footer">

    </div>
</template>

<script>
export default {
    name: 'FooterDC',
    data() {
        return {
            footerLi: [
                {
                    title: 'dc comics',
                    liList: [
                        {
                            text: 'Characters',
                            url: '#'
                        },
                        {
                            text: 'Comics',
                            url: '#'
                        },
                        {
                            text: 'Movies',
                            url: '#'
                        },
                        {
                            text: 'Tv',
                            url: '#'
                        },
                        {
                            text: 'Games',
                            url: '#'
                        },
                        {
                            text: 'Videos',
                            url: '#'
                        },
                        {
                            text: 'News',
                            url: '#'
                        }
                    ]
                },
                {
                    title: 'dc',
                    liList: [
                        {
                            text: 'Terms Of Use',
                            url: '#'
                        },
                        {
                            text: 'Privacy policy (New)',
                            url: '#'
                        },
                        {
                            text: 'Ad Choices',
                            url: '#'
                        },
                        {
                            text: 'Advertising',
                            url: '#'
                        },
                        {
                            text: 'Jobs',
                            url: '#'
                        },
                        {
                            text: 'Subscriptions',
                            url: '#'
                        },
                        {
                            text: 'Talent Workshops',
                            url: '#'
                        },
                        {
                            text: 'CPSC Certificates',
                            url: '#'
                        },
                        {
                            text: 'Ratings',
                            url: '#'
                        },
                        {
                            text: 'Shop Help',
                            url: '#'
                        },
                        {
                            text: 'Contact Us',
                            url: '#'
                        }
                    ]
                },
                {
                    title: 'sites',
                    liList: [
                        {
                            text: 'DC',
                            url: '#'
                        },
                        {
                            text: 'MAD Magazine',
                            url: '#'
                        },
                        {
                            text: 'DC Kids',
                            url: '#'
                        },
                        {
                            text: 'DC Universe',
                            url: '#'
                        },
                        {
                            text: 'DC Power Visa',
                            url: '#'
                        }
                    ]
                },
                {
                    title: 'shop',
                    liList: [
                        {
                            text: 'Shop DC',
                            url: '#'
                        },
                        {
                            text: 'Shop DC Collectibles',
                            url: '#'
                        }
                    ]
                },
            ]
        }
    }
}
</script>

<style lang="scss" scoped></style>