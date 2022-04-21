<template>
  <div>
  <section class="row container">
    <div class="row__left">
      <h1>Restaurant QR Code Menu</h1>
      <p>Scan the QR code to view our menu</p>
    </div>
    <qrcode value="https://www.buffalowildwings.com/en/food/" :options="{
      color: {
        dark: '#FFC72C',
        light: '#DA291C',
      },
      width: 300
    }"></qrcode>
  </section>
    <footer>
      <address>
        &copy; 2022. Built with Nuxt.js
      </address>
    </footer>
  </div>
</template>

<script>
import VueQrcode from "@chenfengyuan/vue-qrcode";
export default {
  components: {
    qrcode: VueQrcode,
  },
};
</script>
