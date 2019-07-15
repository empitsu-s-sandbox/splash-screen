<template>
  <div class="splash-screen">
    <div class="wrap">
      <img src="/25.svg" alt="loading-image">
    </div>
  </div>
</template>
<style lang="scss">
.splash-screen {
  background: #4a596a;
  position: fixed;
  top: 0;
  left: 0;
  bottom: 0;
  right: 0;
  z-index: 99999;
}
.splash-screen > .wrap {
  position: absolute;
  top: 50%;
  left: 50%;
  transform: translateX(-50%) translateY(-50%);
}
.splash-screen > .wrap > img {
  margin: 30px auto;
  display: block;
  width: 150px;
}
.splash-screen > .wrap > img.logo{
  -webkit-filter: drop-shadow(0px 2px 2px rgba(0, 0, 0, 0.3));
  filter: drop-shadow(0px 2px 2px rgba(0, 0, 0, 0.3));
}
</style>
