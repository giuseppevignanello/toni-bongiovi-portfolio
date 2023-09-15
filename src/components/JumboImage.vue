
<script>
import ImageMenu from './ImageMenu.vue';
export default {
    components: {
        ImageMenu
    },
    data() {

        return {}
    }
}
</script>
<template>
    <div class="jumbo_image position-relative">
        <div class="displayBox mt-5" data-aos="zoom" data-aos-easing="ease-in" data-aos-delay="300">
            <ImageMenu></ImageMenu>
        </div>
    </div>
</template>


<style lang="scss" scoped></style>