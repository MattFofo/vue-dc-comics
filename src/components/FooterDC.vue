<template>
    <footer>
        <div class="footer-links-bg">
            <div class="container">
                <div class="footer-links">
                    <ul>
                        <h3>DC COMICS</h3>
                        <li v-for="(link, index) in linksDCComics" :key="index">
                            {{ link.text }}
                        </li>
                        <ul>
                            <h3>SHOP</h3>
                            <li  v-for="(link, index) in linksShop" :key="index">
                                {{ link.text }}
                            </li>
                        </ul>
                    </ul>
                    <ul>
                        <h3>DC</h3>
                        <li v-for="(link, index) in linksDC" :key="index">
                            {{ link.text }}
                        </li>
                    </ul>
                    <ul>
                        <h3>SITES</h3>
                        <li v-for="(link, index) in linksSites" :key="index">
                            {{ link.text }}
                        </li>
                    </ul>
                    <img src="../assets/img/dc-logo-bg.png" alt="">
                </div>
            </div>
        </div>
        <div class="footer-socials-bg">
            <div class="container">
                <div class="footer-socials">
                    <button>join now</button>
                    <div class="socials">
                        <h3>FOLLOW US</h3>
                        <img src="../assets/img/footer-facebook.png" alt="facebook-icon">
                        <img src="../assets/img/footer-periscope.png" alt="periscope-icon">
                        <img src="../assets/img/footer-pinterest.png" alt="pinterest-icon">
                        <img src="../assets/img/footer-twitter.png" alt="twitter-icon">
                        <img src="../assets/img/footer-youtube.png" alt="youtube-icon">
                    </div>
                </div>
            </div>
        </div>
    </footer>    
</template>

<script>
export default {
    name: 'FooterDC',
    data() {
        return {
            linksDCComics: [
                {
                    href: '#',
                    text: 'Characters'

                },
                {
                    href: '#',
                    text: 'Comics'

                },
                {
                    href: '#',
                    text: 'Movies'

                },
                {
                    href: '#',
                    text: 'TV'

                },
                {
                    href: '#',
                    text: 'Games'

                },
                {
                    href: '#',
                    text: 'Videos'

                },
                {
                    href: '#',
                    text: 'News'

                }

            ],
            linksShop: [
                {
                    href: '#',
                    text: 'Shop DC'

                },
                                {
                    href: '#',
                    text: 'Shop DC Collectibles'

                }

            ],
            linksDC: [
                {
                    href: '#',
                    text: 'Term Of Use'

                },
                                {
                    href: '#',
                    text: 'Privacy Policy (New)'

                },
                                {
                    href: '#',
                    text: 'Ad Choiches'

                },
                                {
                    href: '#',
                    text: 'Advertising'

                },
                                {
                    href: '#',
                    text: 'Jobs'

                },
                                {
                    href: '#',
                    text: 'Subscriptions'

                },
                                {
                    href: '#',
                    text: 'Talent Workshops'

                },
                                {
                    href: '#',
                    text: 'CPSC Certificates'

                },
                                {
                    href: '#',
                    text: 'Ratings'

                },
                                {
                    href: '#',
                    text: 'Shop Help'

                },
                                {
                    href: '#',
                    text: 'Contact Us'

                }

            ],
            linksSites: [
                {
                    href: '#',
                    text: 'DC'

                },
                {
                    href: '#',
                    text: 'MAD Magazine'

                },
                {
                    href: '#',
                    text: 'DC Kids'

                },
                {
                    href: '#',
                    text: 'DC Universe'

                },
                {
                    href: '#',
                    text: 'DC Power Visa'

                }

            ]
        }
    }
}
</script>

<style scoped lang="scss">
    .footer-links-bg {
        background-image: url('../assets/img/footer-bg.jpg');
        background-size: cover;
        height: 400px;
        overflow: hidden;
        position: relative;
        .footer-links {
            display: flex;
            justify-content: space-evenly;
            img {
                position: relative;
                bottom: 60px;
                margin-left: 16rem;
            }
        }
    }
    .footer-socials-bg {
        background-color: darkgrey;
    }
    .footer-socials {
        display: flex;
        justify-content: space-between;
        .socials {
            display: flex;
            align-items: center;
            gap: 1rem;
        }
    }

</style>