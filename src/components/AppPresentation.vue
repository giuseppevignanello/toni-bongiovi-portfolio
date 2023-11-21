
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
        <div class="d-flex justify-content-center">
            <h1 id="title_name" class="display-1 p-2"> Toni Bongiovì </h1>
        </div>
        <div class=" jumbotron d-flex align-items-center justify-content-between gap-3">
            <JumboBanner></JumboBanner>
            <JumboTextContainer></JumboTextContainer>
            <JumboImage class="col-5 col-xl-4"></JumboImage>
        </div>



    </div>
</template>


<style lang="scss" scoped></style>