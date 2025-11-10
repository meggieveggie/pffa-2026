<script setup lang="ts">
const open_call = new URL('../assets/2026OpenCall.png', import.meta.url).href;
import { BContainer, BRow, BCol, BButton, BImg } from 'bootstrap-vue-3';
const pffaLogo = new URL('../assets/pffa_logo.png', import.meta.url).href
const footerlogo = new URL('../assets/footer.png', import.meta.url).href
const dates = new URL('../assets/2026_dates.png', import.meta.url).href
const background = new URL('../assets/background.png', import.meta.url).href
</script>

<template>
  <b-container 
    fluid 
    class="d-flex flex-column min-vh-100 px-0 **view-background**"
    :style="{ backgroundImage: 'url(' + background + ')' }" 
  >
  <b-row>
    <b-col xs="12" lg="6" class="mt-5">
      <b-row  class="mt-5">
        <b-img :src="pffaLogo"></b-img>
      </b-row>
    </b-col>
<b-col xs="12" lg="4" class="mt-5 d-flex flex-column justify-content-end">
    <b-row>
        <b-img fluid :src="dates"></b-img>
    </b-row>
    
</b-col>
  </b-row>
  <b-img :src="footerlogo"  class="footer-image" fluid></b-img>
</b-container>

</template>

<style scoped>

.view-background {
  background-size: cover;          /* Ensures the image covers the entire element */
  background-position: center center; /* Centers the image */
  background-repeat: no-repeat;    /* Prevents tiling */
  background-attachment: scroll;
  
}

.custom-button-width {
  width: 350px; /* Adjust this value as needed for your desired fixed width */
}

.custom-button-width {
  width: 350px; /* Adjust this value as needed for your desired fixed width */
}

@media (max-width: 576px) {
  .move-image-right{
    margin-left: 50px; /* Adjust the value as needed */
  }
}

/* Footer styles */
.footer-image {
  width: 100%;
  margin-top: auto;
  margin-bottom: 0px;
}

.form-button {
  background-color: #D9D9D9 !important;
  border-color: #D9D9D9 !important;
  color: black !important;
  font-weight: bold !important;
}
</style>