
<script>
import AppPresentation from "./components/AppPresentation.vue";
import AOS from "aos";
export default {
  data() {
    components: {
      AppPresentation;
    }
    ;
    return {};
  }, mounted() {
    AOS.init();
  },
  components: { AppPresentation }
}
</script>

<template>
  <AppPresentation></AppPresentation>
  <div class="displayBox mt-5" data-aos="slide-right" data-aos-easing="ease-in">

    <div class="box">
      <h1 class="text-center mt-5">Qua ci vanno alcuni quadri</h1>
    </div>
  </div>


  <div class="displayBox mt-5" data-aos="slide-up" data-aos-easing="ease-in">

    <div class="box">
      <h1 class="text-center mt-5">Qua ci mettiamo altri quadri</h1>
    </div>
  </div>
  <footer class="bg-dark">
    <h5 class="text-center text-white mt-5 py-3">Footer</h5>
  </footer>
</template>


<style lang="scss" scoped></style>