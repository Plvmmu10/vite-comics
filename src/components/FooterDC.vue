<template>
    <div class="myContainer">
        <div class="top-footer text-white d-flex justify-content-between">
            <div class="listContainer d-flex flex-wrap">
                <ul v-for="(item, index) in footerLi" :key="index" class="d-flex flex-column">
                    <h4 class="text-uppercase m-0">{{ item.title }}</h4>

                    <ul class="d-flex flex-column p-0">
                        <li v-for="(obj, i) in item.liList" :key="i" class="listItem">
                            <a>
                                {{ obj.text }}
                            </a>
                        </li>
                    </ul>

                </ul>
            </div>

            <div class="img-box">
            </div>
        </div>


    </div>

    <div class="bottom-footer d-flex justify-content-center">
        <div class="w-75 d-flex justify-content-between">
            <div>
                <button class="text-uppercase fw-bold">sign-up now!</button>
            </div>

            <div class="d-flex align-items-center flex-wrap">
                <h4 class="text-uppercase m-0 px-3">follow us</h4>

                <img src="/images/footer-facebook.png" alt="facebook">
                <img src="/images/footer-twitter.png" alt="twitter">
                <img src="/images/footer-youtube.png" alt="twitter">
                <img src="/images/footer-pinterest.png" alt="twitter">
                <img src="/images/footer-periscope.png" alt="twitter">
            </div>
        </div>
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

<style lang="scss" scoped>
.myContainer {
    margin: 0 auto;
    padding: 0;
}

.top-footer {
    width: 100%;

    .img-box {
        width: 75%;
        background-image: url(/images/dc-logo-bg.png);
        background-repeat: no-repeat;
        background-position: center;

        img {
            object-fit: cover;
            width: 100%;
        }
    }

}

.listContainer {
    padding: 2rem 0;
    width: 37%;

    ul {
        padding: 0 .1;
        margin: 0;

        .listItem {
            color: rgba(211, 211, 211, 0.5);
        }
    }
}

.bottom-footer {
    width: 100%;
    margin: 0 auto;
    padding: 2rem 0;
    background-color: #303030;
    color: #0282f9;

    button {
        background-color: transparent;
        border: 2px solid #0282f9;
        color: white;
        padding: .5rem;
    }

    img {
        padding: 0 .5rem;
    }
}
</style>