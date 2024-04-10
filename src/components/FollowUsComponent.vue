<template>
    <div class="fd-followUs-style">
        <div class="container d-flex justify-content-between">
            <div>

            </div>
            <div class="position-relative cropped">
                <img src="../../public/img/dc-logo-bg.png" alt="DC-Background-image">
            </div>
        </div>
    </div>
</template>

<script>
export default {
    name: 'FollowUsComponent',
    data() {
        return {

        }
    }
}
</script>

<style lang="scss" scoped>
.fd-followUs-style {
    height: 45vh;
    background-image: url('../../public/img/footer-bg.jpg');
    background-size: cover;
}

img {
    position: absolute;
    right: 0;
    top: -80px;
}

.cropped {
    width: 600px;
    height: 45vh;
    overflow: hidden;
}

</style>