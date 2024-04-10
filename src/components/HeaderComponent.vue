<template>
    <div class="container d-flex justify-content-between bg-white">
        <div class="d-flex align-items-center justify-content-center">
            <img src="../../public/img/dc-logo.png" alt="Logo-Header">
        </div>
        <div>
            <ul class="d-flex align-items-center justify-content-center gap-5 list-unstyled ">
                <li class="text-uppercase fw-bold text-black" v-for="link in links" :key="link">{{ link }}
                    
                </li>
            </ul>
        </div>
    </div>
</template>

<script>
    export default {
        name: 'HeaderComponent',
        data() {
            return {
                links: ['CHARACTERS', 'COMICS', 'MOVIES', 'TV', 'GAMES', 'COLLECTIBLES', 'VIDEOS', 'FANS', 'NEWS', 'SHOP']
            }
        },
        
    }
</script>

<style lang="scss" scoped>
    .container {
        height: 100px;
    }

    img{
        width: 80px;
        height: 80px;
    }

    ul {
        line-height: 100px;
    }

    li {
        cursor: pointer;
    }
</style>