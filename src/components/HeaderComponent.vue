<template>
    <div class="container d-flex justify-content-between bg-white">
        <div class="d-flex align-items-center justify-content-center">
            <img src="../../public/img/dc-logo.png" alt="Logo-Header">
        </div>
        <div>
            <ul class="d-flex align-items-center justify-content-center gap-5 list-unstyled  ">
                <li class="text-uppercase fw-bold text-black" v-for="(link, index) in links" :key="index">
                    <a href="#" class="text-decoration-none text-black">{{ link.name }}</a>
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
                links: [
                    {
                        name : 'CHARACTERS',
                        url : '#'
                    },
                    {
                        name : 'COMICS',
                        url : '#'
                    },
                    {
                        name : 'MOVIES',
                        url : '#'
                    },
                    {
                        name : 'TV',
                        url : '#'
                    },
                    {
                        name : 'GAMES',
                        url : '#'
                    },
                    {
                        name : 'COLLECTIBLES',
                        url : '#'
                    },
                    {
                        name : 'VIDEOS',
                        url : '#'
                    }
                ]
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

</style>