<template>
    <div class="fd-footer-style">
        <div class="container">
            <div>
                <button class="fd-button">SIGN-UP NOW!</button>
            </div>
            <div class="fd-style">
                <ul class="d-flex align-items-center justify-content-center gap-3 list-unstyled">
                    <h2>FOLLOW US</h2>
                    <li v-for="(item, index) in arrayFontAwesome" :key="index">
                        <a :href="item.url"><i class="fs-3" :class="item.name"></i></a>
                    </li>
                </ul>
            </div>
        </div>

    </div>
</template>

<script>
export default {
    name: 'FooterComponent',
    data() {
        return {
            arrayFontAwesome: [
                {
                    name: 'fab fa-facebook-f',
                    url: '#'
                },
                {
                    name: 'fab fa-twitter',
                    url: '#'
                },
                {
                    name: 'fab fa-youtube',
                    url: '#'
                },
                {
                    name: 'fab fa-pinterest-p',
                    url: '#'
                },
                {
                    name: 'fab fa-periscope',
                    url: '#'
                }
            ]
        }
    }
}
</script>

<style lang="scss" scoped>
@use '../assets/styles/partials/variables' as *;

.fd-footer-style {
    height: 100px;
    background-color: #303030;
}

.fd-style {
    padding-top: 10px
}


.container {
    height: 100px;
    display: flex;
    align-items: center;
    align-content: center;
    justify-content: space-between;
}

.fd-button {
    background-color: #303030;
    color: white;
    border: 2px solid $maincolor;
    padding: 10px 10px;
    margin: auto 0;

    &:hover {
        background-color: $maincolor;
        color: white;
    }
}

li {
    background-color: $textcolor;
    width: 50px;
    height: 50px;
    border-radius: 50%;
    display: flex;
    justify-content: center;
    align-items: center;
    &:hover {
        background-color: white;
        cursor: pointer;
    }
}

a {
    text-decoration: none;
}

h2 {
    color: $maincolor;
    font-size: 20px;
    margin: auto 0;
    &:hover {
        color: white;
        cursor: pointer;
    }
}
</style>