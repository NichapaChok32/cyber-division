<template>
  <div class="bg">
    <div class="container"></div>
  </div>
  <div id="App">
    <navbar></navbar>
    <client-only>
      <main-banner> </main-banner>
      <simple-solutions></simple-solutions>
      <empowered></empowered>
      <our-teams></our-teams>
    </client-only>
    <footers></footers>
  </div>
</template>

<script setup>
useHead({
  title: "Cyber Division",
});
</script>

<style>
@import url("https://rsms.me/inter/inter.css");
@import url("./assets/css/fonts.css");
body {
  background-color: #021b04;
  margin: 0;
  overflow-x: hidden;
}

@media screen and (max-width: 990px) {
  body {
    width: 100%;
    margin: 0 auto;
  }
}

.bg {
  position: fixed;
  top: -50%;
  left: -50%;
  right: -50%;
  bottom: -50%;
  width: 200%;
  height: 200vh;
  background: transparent url("./assets/images/noise.gif") repeat 0 0;
  background-repeat: repeat;
  animation: bg-animation 0.2s infinite;
  opacity: 0.9;
  visibility: visible;
  mix-blend-mode: screen;
}

#App {
  width: 100%;
  height: 100vh;
  margin: 0 auto;
  opacity: 1;
}

@keyframes bg-animation {
  0% {
    transform: translate(0, 0);
  }
  10% {
    transform: translate(-5%, -5%);
  }
  20% {
    transform: translate(-10%, 5%);
  }
  30% {
    transform: translate(5%, -10%);
  }
  40% {
    transform: translate(-5%, 15%);
  }
  50% {
    transform: translate(-10%, 5%);
  }
  60% {
    transform: translate(15%, 0);
  }
  70% {
    transform: translate(0, 10%);
  }
  80% {
    transform: translate(-15%, 0);
  }
  90% {
    transform: translate(10%, 5%);
  }
  100% {
    transform: translate(5%, 0);
  }
}
</style>
