<template>
    <div class="myContainer">

        <!-- Top footer with all lists and big logo -->
        <div class="top-footer text-white d-flex justify-content-between">

            <!-- List container -->
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

            <!-- Big logo container -->
            <div class="img-box">
            </div>
        </div>


    </div>

    <!-- Bottom footer with sign-up button and social icons -->
    <div class="bottom-footer d-flex justify-content-center">
        <div class="w-75 d-flex justify-content-between">
            <!-- Sign up button -->
            <div>
                <button class="text-uppercase fw-bold btn btn-outline-primary">sign-up now!</button>
            </div>

            <div class="d-flex align-items-center flex-wrap">
                <h4 class="text-uppercase m-0 px-3">follow us</h4>

                <!-- All social icons -->
                <img src="/images/footer-facebook.png" alt="facebook">
                <img src="/images/footer-twitter.png" alt="twitter">
                <img src="/images/footer-youtube.png" alt="youtube">
                <img src="/images/footer-pinterest.png" alt="pinterest">
                <img src="/images/footer-periscope.png" alt="periscope">
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
        width: 70%;
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
    width: 40%;

    ul {
        padding: 10px;
        margin: 0;

        .listItem {
            color: rgba(211, 211, 211, 0.5);
            cursor: pointer;

            a:hover {
                color: #0282f9;
            }
        }
    }
}

.bottom-footer {
    width: 100%;
    margin: 0 auto;
    padding: 2rem 0;
    background-color: #303030;
    color: #0282f9;

    img {
        padding: 0 .5rem;
        cursor: pointer;
    }
}
</style>