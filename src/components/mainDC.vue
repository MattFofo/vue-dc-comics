<template>
<div class="container">
    <div class="main-grid"></div>
    <div class="main-banner">
        <div v-for="(link, index) in bannerLinks" :key="index">
        <a :href="link.href">
            <img :src="'../assets/img/' + link.img" :alt="link.text">
            <div>{{ link.text }}</div>    
        </a>
        </div>
    </div>
</div>
  
</template>

<script>
export default {
    name: 'mainDC',
    data() {
        return {
            bannerLinks: [
                {
                    href: '#',
                    img: 'buy-comics-digital-comics.png',
                    text: 'DIGITAL COMICS',
                },
                {
                    href: '#',
                    img: 'buy-comics-merchandise.png',
                    text: 'DC MERCHANDISE',
                },
                {
                    href: '#',
                    img: 'buy-comics-subscription.png',
                    text: 'SUBSCRIPTION',
                },
                {
                    href: '#',
                    img: 'buy-comics-shop-locator.png',
                    text: 'COMIC SHOP LOCATOR',
                },
                {
                    href: '#',
                    img: 'buy-dc-power-visa.png',
                    text: 'DC POWER VISA',
                }
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