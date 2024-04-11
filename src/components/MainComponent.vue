<template>
    <div class="fd-style">
        <ul class="container d-flex align-items-center justify-content-between">
            <li v-for="(object, index) in objects" :key="index" class="d-flex align-items-center gap-3">
                <img :src="object.src" :alt="object.alt">
                <p>{{ object.text }}</p>
            </li>
        </ul>
    </div>
</template>

<script>
export default {
    name: 'MainComponent',

    data() {
        return {
            objects: [
                {
                    src: '../../public/img/buy-comics-digital-comics.png',
                    alt: 'digital-comics',
                    text: 'DIGITAL COMICS'
                },

                {
                    src: '../../public/img/buy-comics-merchandise.png',
                    alt: 'merchandise',
                    text: 'DC MERCHANDISE'
                },

                {
                    src: '../../public/img/buy-comics-subscriptions.png',
                    alt: 'subscriptions',
                    text: 'SUBSCRIPTION'
                },

                {
                    src: '../../public/img/buy-comics-shop-locator.png',
                    alt: 'shop-locator',
                    text: 'COMIC SHOP LOCATOR'
                },

                {
                    src: '../../public/img/buy-dc-power-visa.svg',
                    alt: 'power-visa',
                    text: 'DC POWER VISA'
                }

            ]
        }
    }
}
</script>
<!-- Cambiare tutte le altezze in pixel e non piu vh -->
<style lang="scss" scoped>
@use '../assets/styles/partials/variables' as *;
.fd-style {
    height: 150px;
    background-color: $maincolor;
}

.container {
    height: 150px;
    background-color: $maincolor;
}

img {
    width: 40px;
    height: 50px;
    &:hover {
        filter: invert(1);
        cursor: pointer;
    }
}

p {
    color: white;
    margin: 0 auto;
    &:hover {
        filter: invert(1);
        cursor: pointer;
    }
}
</style>