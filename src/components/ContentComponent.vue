<template>
    <div class="fd-height bg-black">
        <div class="container">
            <p> --> Content Goes Here <-- </p>
        </div>
    </div>
</template>

<script>
export default {
    name: 'ContentComponent',
    data() {
        return {

        }
    }
}
</script>

<style lang="scss" scoped>
.fd-height {
    height: 100px;
}
.container {
    height: 100px;
    background-color: black;
}

p {
    line-height: 100px;
    color: white;
    font-size: 30px;
}
</style>