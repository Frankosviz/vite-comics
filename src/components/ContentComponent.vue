<template>
    <div class="bg-black">
        <div class="container bg-black">
            <button class="fd-current-series-btn">CURRENT SERIES</button>
            <div class="pt-5">
                <CardComponent />
            </div>
            <div class="d-flex justify-content-center pt-5 pb-5">
                <button class="fd-button">
                    LOAD MORE
                </button>
            </div>
        </div>
    </div>
</template>

<script>
import CardComponent from './CardComponent.vue';
export default {
    name: 'ContentComponent',
    components: { CardComponent },
    data() {
        return {
        };
    },
}
</script>

<style lang="scss" scoped>
@use '../assets/styles/partials/variables' as *;

.fd-button {
    text-align: center;
    font-weight: bold;
    background-color: $maincolor;
    width: 300px;
    height: 40px;
    color: white;
    border: 2px solid $maincolor;

    &:hover {
        background-color: white;
        color: $maincolor;
        cursor: pointer;
    }
}

.fd-current-series-btn {
    text-align: center;
    font-weight: bold;
    background-color: $maincolor;
    width: 200px;
    height: 40px;
    color: white;
    border: 2px solid $maincolor;
    font-size: 20px;
    transform: translate(0, -50%);

    &:hover {
        background-color: white;
        color: $maincolor;
        cursor: pointer;
    }
}

// .fd-height {
//     height: 500px;
// }
// .container {
//     height: 500px;
//     background-color: black;
// }
</style>