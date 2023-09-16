
<script>
import AppPresentation from "./components/AppPresentation.vue";
import AOS from "aos";
import AppHeader from "./components/AppHeader.vue"
export default {
  data() {

    return {
      images: [
        { url: '../public/img/acrilico_tela.png', alt: 'Image 1' },
        { url: '../public/img/modena.png', alt: 'Image 2' },
        { url: '../public/img/sabbia_acrilico_1.png', alt: 'Image 3' },

      ],
      currentIndex: 0,
      timer: null,
    };
  },
  components: { AppPresentation, AppHeader },
  methods: {
    startCarousel() {
      this.timer = setInterval(() => {
        this.nextSlide();
      }, 1200);
    },
    stopCarousel() {
      clearInterval(this.timer);
      this.timer = null;
    },
    nextSlide() {
      this.currentIndex = (this.currentIndex + 1) % this.images.length;
    },
  }, mounted() {
    AOS.init();
    this.startCarousel();
  },
  beforeDestroy() {
    this.stopCarousel();
  },
}
</script>

<template>
  <AppHeader></AppHeader>
  <AppPresentation></AppPresentation>
  <div class="displayBox mt-5" data-aos="slide-right" data-aos-easing="ease-in">

    <div class="box">
      <div class="carousel">
        <div class="carousel-inner">
          <div class="carousel-item" :class="{ active: currentIndex === index }" v-for="(image, index) in images"
            :key="index">
            <img :src="image.url" :alt="image.alt" />
          </div>
        </div>
      </div>
    </div>
  </div>

  <div class="CTA">
    <h3 class="text-center pt-3">Ti piacciono le mie opere?</h3>
    <h2 class="text-center">Puoi comprarle!</h2>
    <div class="d-flex justify-content-center">
      <button type="button" class="btn btn-success">Contattami</button>
    </div>
  </div>


  <div class="displayBox mt-5" data-aos="slide-up" data-aos-easing="ease-in">

    <div class="box">
      <h1>I miei quadri</h1>
    </div>
  </div>
  <footer class="bg-dark">
    <h5 class="text-center text-white mt-5 py-3">Footer</h5>
  </footer>
</template>


<style lang="scss" scoped></style>