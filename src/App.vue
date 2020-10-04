<template>
  <div id="app">
    <router-view />
  </div>
</template>


<style>
  @font-face {
    font-family: "Druk";
    src: local("Druk"),
    url(./assets/fonts/druk/DrukTextWide-Bold.woff) format("woff"),
    url(./assets/fonts/druk/DrukTextWide-Bold.woff2) format('woff2'), /* Super Modern Browsers */
       url(./assets/fonts/druk/DrukTextWide-Bold.ttf)  format('truetype'); /* Safari, Android, iOS */
  }

   @font-face {
    font-family: "Syne";
    src: local("Syne"),
    url(./assets/fonts/syne/Syne-Regular.woff) format("woff"),
    url(./assets/fonts/syne/Syne-Regular.woff2) format('woff2'); /* Super Modern Browsers */
  }
</style>