<template>
<main>
    <div class="main-grid"></div>
    <div class="main-banner">
    <div class="container">
        <div class="banner" v-for="(link, index) in bannerLinks" :key="index">
            <img :src="link.img" :alt="link.text">
            <a :href="link.href">
                <div>{{ link.text }}</div>    
            </a>
        </div>
    </div>
</div>
</main>
</template>

<script>
import img1 from '../assets/img/buy-comics-digital-comics.png';
import img2 from '../assets/img/buy-comics-merchandise.png';
import img3 from '../assets/img/buy-comics-shop-locator.png';
import img4 from '../assets/img/buy-comics-subscriptions.png';
import img5 from '../assets/img/buy-dc-power-visa.svg';
export default {
    name: 'MainDC',
    data() {
        return {
            bannerLinks: [
                {
                    href: '#',
                    img: img1,
                    text: 'DIGITAL COMICS',
                },
                {
                    href: '#',
                    img: img2,
                    text: 'DC MERCHANDISE',
                },
                {
                    href: '#',
                    img: img3,
                    text: 'SUBSCRIPTION',
                },
                {
                    href: '#',
                    img: img4,
                    text: 'COMIC SHOP LOCATOR',
                },
                {
                    href: '#',
                    img: img5,
                    text: 'DC POWER VISA',
                }
            ]
        }
    }
}
</script>

<style scoped lang="scss">
@import '../assets/styles/partials/variables.scss';
@import '../assets/styles/partials/general.scss';
    .main-grid {
        height: 6rem;
        background-color: $secondaryColor;
    }
    .main-banner {
        text-align: center;
        background-color: $primaryColor;
        .container {
            display: flex;
            justify-content: space-between;
        }
        .banner {
            display: flex;
            align-items: center;
        }
        div {
            display: inline-block;
        }        
        img {
            width: 4rem;
            height: 5rem;
            object-fit: contain;
        }
    }

</style>