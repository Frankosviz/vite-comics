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
    height: 10vh;
}
.container {
    height: 10vh;
    background-color: black;
}

p {
    line-height: 10vh;
    color: white;
    font-size: 30px;
}
</style>