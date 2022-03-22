<template>
    <header>
    <div class="container">
        <img src="../assets/img/dc-logo.png" alt="">
        <ul>
            <li v-for="(link, index) in links" :key="index">
                <a :href="link.href">
                    {{ link.text }}
                </a>
            </li>
        </ul>
    </div>
    </header>
</template>

<script>
export default {
    name: 'HeaderDC',
    data() {
        return {
            links: [
                {
                    href: '#',
                    text: 'CHARACTERS'
                },
                {
                    href: '#',
                    text: 'COMICS'
                },
                {
                    href: '#',
                    text: 'MOVIES'
                },
                {
                    href: '#',
                    text: 'TV'
                },
                {
                    href: '#',
                    text: 'GAMES'
                },
                {
                    href: '#',
                    text: 'COLLECTIBLES'
                },
                {
                    href: '#',
                    text: 'VIDEOS'
                },
                {
                    href: '#',
                    text: 'FANS'
                },
                {
                    href: '#',
                    text: 'NEWS'
                },
                {
                    href: '#',
                    text: 'SHOP'
                },
                
            ]
        }
    }
}
</script>

<style scoped lang="scss">
    header {
        .container {
        display: flex;
        justify-content: space-between;
        align-items: center;
        }
    }
    li {
        display: inline-block;
        padding: 1rem;
        a {
            text-decoration: none;
        }
    }
</style>