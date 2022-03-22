<template>
<div class="container">
    <div class="main-grid"></div>
    <div class="main-banner">
        <div>
        <a v-for="(link, index) in bannerLinks" :key="index" :href="link.href">
            <img :src="link.img" :alt="link.text">
            <div>{{ link.text }}</div>    
        </a>
        <a href="">
            <img src="../assets/img/buy-dc-power-visa.svg" alt="">
            <div>DC POWER VISA</div>
        </a>
        </div>
    </div>
</div>
  
</template>
<script>
import img1 from '../assets/img/buy-comics-digital-comics.png';
import img2 from '../assets/img/buy-comics-merchandise.png';
import img3 from '../assets/img/buy-comics-shop-locator.png';
import img4 from '../assets/img/buy-comics-subscriptions.png';
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
            ]
        }
    }
}
</script>

<style scoped lang="scss">
@import '../assets/styles/partials/variables.scss';
    .main-grid {
        height: 6rem;
        background-color: $secondaryColor;
    }
    .main-banner {
        background-color: $primaryColor;
    }

</style>