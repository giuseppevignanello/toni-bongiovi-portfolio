
<script>
import JumboBanner from './JumboBanner.vue';

export default {
    components: {
        JumboBanner
    },
    data() {
        return {};
    },
    components: { JumboBanner }
}
</script>

<template>
    <div>
        <h1 id="title_name" class="text-white text-center">Toni <strong>Bongiovì</strong> </h1>
        <div class="displayBox" data-aos="slide-left" data-aos-easing="ease-in">
            <div>
                <div class="jumbotron d-flex mt-5">
                    <JumboBanner></JumboBanner>
                    <div class="jumbo_text_container d-flex flex-column justify-content-around">
                        <div>
                            <h2 id="saluto" class="mt-5">Ciao!</h2>
                            <p id="jumbo_text" class="mt-4">Sono un artista e insegnante siciliano. Vivo e lavoro a Modena
                            </p>
                        </div>

                        <div class="socials d-flex gap-2 justify-content-center mt-3">
                            <div>
                                <i class="fa-brands fa-facebook fa-xl"></i>
                            </div>
                            <div>
                                <i class="fa-brands fa-instagram fa-xl"></i>
                            </div>
                        </div>
                    </div>

                    <div class="jumbo_image position-relative">
                        <div class="image_menu d-flex gap-2">
                            <div>
                                <i class="fa-solid fa-address-card fa-xl"></i>
                            </div>
                            <div>
                                <i class="fa-solid fa-paintbrush fa-xl"></i>
                            </div>
                            <div>
                                <i class="fa-solid fa-message fa-xl"></i>
                            </div>
                        </div>
                    </div>
                </div>
            </div>

        </div>
    </div>
</template>


<style lang="scss" scoped></style>