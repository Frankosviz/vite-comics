<template>
    <div class="bg-black">
        <div>
            <CardComponent />
        </div>
    </div>
</template>

<script>
import CardComponent from './CardComponent.vue';
export default {
    name: 'ContentComponent',
    components:  {CardComponent}, 
    data() {
        return {
        };
    },    
}
</script>

<style lang="scss" scoped>
// .fd-height {
//     height: 500px;
// }
// .container {
//     height: 500px;
//     background-color: black;
// }
</style>