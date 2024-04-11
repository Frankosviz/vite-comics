<template>
    <div class="fd-hero-style">

    </div>
</template>

<script>
    export default {
        name: 'HeroComponent',
        data(){
            return {

            }
        }
        
    }
</script>

<style lang="scss" scoped>
    @use '../assets/styles/partials/variables' as *;
    .fd-hero-style {
        height: 400px;
        background-image: url('../../public/img/jumbotron.jpg');
        background-size: cover;
    }
</style>