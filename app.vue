<template>
  <div>
    <section id="introduction" class="sec">
      <Navigation />

      <Header />
    </section>
    <div class="zero">
      <Caraousel />
      <Services />
    </div>
  </div>
</template>

<script setup>
import Caraousel from "~/components/Caraousel.vue";
import Navigation from "~/components/Navigation.vue";
import Header from "~/components/Header.vue";
import Services from "~/components/Services.vue";
</script>

<style>
@import url('https://fonts.googleapis.com/css2?family=Nunito+Sans:wght@300;400&display=swap');


body {
  font-family: 'Nunito Sans';
  margin: 0;
  padding: 0;
  box-sizing: border-box;
  background-color: #f4f5f7;
}
.zero {
  background-color: #fcfcfc;
}
.sec{
  min-height: 100vh;
}
</style>
