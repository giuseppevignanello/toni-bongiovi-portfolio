
<script>
import JumboBanner from './JumboBanner.vue';
import JumboTextContainer from './JumboTextContainer.vue';
import JumboImage from './JumboImage.vue';
export default {
    data() {
        return {};
    },
    components: { JumboBanner, JumboTextContainer, JumboImage }
}
</script>

<template>
    <div>
        <h1 id="title_name" class="text-white text-center">Toni <strong>Bongiovì</strong> </h1>
        <div class="displayBox" data-aos="slide-left" data-aos-easing="ease-in">
            <div class="jumbotron_background">
                <div class="jumbotron d-flex mt-5">
                    <JumboBanner></JumboBanner>
                    <JumboTextContainer></JumboTextContainer>
                    <JumboImage></JumboImage>
                </div>
            </div>

        </div>
    </div>
</template>


<style lang="scss" scoped></style>