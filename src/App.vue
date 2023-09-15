
<script>
import AOS from "aos";
export default {
  data() {


    return {}
  }, mounted() {
    AOS.init()
  },
}
</script>

<template>
  <div class="bg">
    <h1 id="title_name" class="text-white text-center">Toni <strong>Bongiovì</strong> </h1>
    <div class="displayBox" data-aos="slide-left" data-aos-easing="ease-in">
      <div>
        <div class="jumbotron d-flex mt-5">
          <div class="left_banner">
            <ul class="list-unstyled d-flex flex-column justify-content-around align-items-center h-100">
              <li class="text-vertical text-white">MURALES </li>
              <li class="text-vertical text-white">QUADRI IN SABBIA </li>
              <li class="text-vertical text-white">SURREALISMO </li>
            </ul>
          </div>
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
    <div class="bg">
      <div class="displayBox mt-5" data-aos="slide-right" data-aos-easing="ease-in">

        <div class="box">
          <h1 class="text-center mt-5">Qua ci vanno alcuni quadri</h1>
        </div>
      </div>
    </div>
    <div class="bg">
      <div class="displayBox mt-5" data-aos="slide-left" data-aos-easing="ease-in">

        <div class="box">
          <h1 class="text-center mt-5">Qua ci mettiamo altri quadri</h1>
        </div>
      </div>
    </div>
    <footer class="bg-dark">
      <h5 class="text-center text-white mt-5 py-3">Footer</h5>
    </footer>
  </div>
</template>


<style lang="scss" scoped></style>