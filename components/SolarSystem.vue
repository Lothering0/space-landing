<template>
  <div class="solar-system">
    <div class="ring ring-1"></div>
    <div class="ring ring-2"></div>
    <div class="ring ring-3"></div>
    <div class="ring ring-4"></div>
    <div class="ring ring-5"></div>
    <div class="ring ring-6"></div>
    <div class="ring ring-7"></div>
    <div class="ring ring-8"></div>
    <div class="sun"></div>
  </div> 
</template>

<style lang="scss" scoped>
.solar-system {
  position: relative;

  width: 2054px;
  height: 2054px;

  padding-top: 28px;
  left: -825px;

  background-image: radial-gradient(
    50% 50% at 50% 50%,
    rgba(255, 230, 0, 0.34) 0%,
    rgba(196, 196, 196, 0) 100%,
    rgba(255, 255, 255, 0) 100%
  );
}

.sun, .ring {
  position: absolute;

  top: 50%;
  left: 50%;

  transform: translate(-50%, -50%);
}

.sun {
  width: 512px;
  height: 512px;

  background-image: url('@/static/sun.png');
}

.ring {
  border: 11px solid #fff;
  border-radius: 50%;
}

.ring-1 {
  width: 771px;
  height: 771px;
}

.ring-2 {
  width: 952px;
  height: 952px;
}

.ring-3 {
  width: 1133px;
  height: 1133px;
}

.ring-4 {
  width: 1314px;
  height: 1314px;
}

.ring-5 {
  width: 1495px;
  height: 1495px;
}

.ring-6 {
  width: 1676px;
  height: 1676px;
}

.ring-7 {
  width: 1857px;
  height: 1857px;
}

.ring-8 {
  width: 2038px;
  height: 2038px;
}
</style>
