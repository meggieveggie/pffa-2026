<script setup lang="ts">
const open_call = new URL('../assets/2026OpenCall.png', import.meta.url).href;
import { BContainer, BRow, BCol, BButton, BImg } from 'bootstrap-vue-3';
const pffaLogo = new URL('../assets/pffa_logo.png', import.meta.url).href
const footerlogo = new URL('../assets/footer.png', import.meta.url).href
</script>

<template>
  <b-container fluid class="d-flex flex-column min-vh-100 px-0">
  <b-row>
    <b-col xs="12" lg="5" class="mt-5">
      <b-row  class="mt-5">
        <b-img :src="pffaLogo"></b-img>
      </b-row>
    </b-col>
    <b-col xs="12" lg="6" class="mt-5 d-flex flex-column justify-content-end">
    <b-col cols="12" md="10" lg="8"> <b-img fluid :src="open_call"></b-img>
        </b-col>
      <b-col lg="12" class="mb-3 mt-5">
          <BButton 
          href="https://docs.google.com/forms/d/e/1FAIpQLSeAjfKhSVVytf5HWj9Cm18JZ4zcNBzi_AKsChqzrv5c3oGiAg/viewform?usp=sharing&ouid=112398555283612625022" 
          variant="light"
          class="form-button not-bold move-right custom-button-width"
          size="lg"
          target="_blank"
          rel="noopener noreferrer"
          >Submit your film</BButton>
        </b-col>

        <b-col lg="12" class="mb-3">
          <BButton 
          href="https://docs.google.com/forms/d/e/1FAIpQLSeAjfKhSVVytf5HWj9Cm18JZ4zcNBzi_AKsChqzrv5c3oGiAg/viewform?usp=sharing&ouid=112398555283612625022" 
          variant="light"
          class="form-button not-bold move-right custom-button-width"
          size="lg"
          target="_blank"
          rel="noopener noreferrer"
          >Submit your performance</BButton>
        </b-col>

        <b-col lg="12" class="mb-3">
          <BButton 
          href="https://docs.google.com/forms/d/e/1FAIpQLSerQPleNLIbmRj2GNmHdJN_n3y9s-ZQp8GyzroWEkTXdOzu5w/viewform?usp=sharing&ouid=112398555283612625022" 
          variant="light"
          class="form-button not-bold move-right custom-button-width"
          size="lg"
          target="_blank"
          rel="noopener noreferrer"
          >Submit your workshop </BButton>
        </b-col>
    </b-col>
  </b-row>
  <b-img :src="footerlogo"  class="footer-image" fluid></b-img>
</b-container>

</template>

<style scoped>

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