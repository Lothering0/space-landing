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

    <a
      class="sun"
      href="#start"
      v-scroll-to="{
        el: '#start',
        offset: -51
      }"
      title="Sun"
    ></a>

    <a
      class="planet mercury"
      href="#mercury"
      v-scroll-to="'#mercury'"
      title="Mercury"
    ></a>
    <a
      class="planet venus"
      href="#venus"
      v-scroll-to="'#venus'"
      title="Venus"
    ></a>
    <a
      class="planet earth"
      href="#earth"
      v-scroll-to="'#earth'"
      title="Earth"
    ></a>
    <a
      class="planet mars"
      href="#mars"
      v-scroll-to="'#mars'"
      title="Mars"
    ></a>
    <a
      class="planet jupiter"
      href="#jupiter"
      v-scroll-to="'#jupiter'"
      title="Jupiter"
    ></a>
    <a
      class="planet saturn"
      href="#saturn"
      v-scroll-to="'#saturn'"
      title="Saturn"
    ></a>
    <a
      class="planet uranus"
      href="#uranus"
      v-scroll-to="'#uranus'"
      title="Uranus"
    ></a>
    <a
      class="planet neptune"
      href="#neptune"
      v-scroll-to="'#neptune'"
      title="Neptune"
    ></a>
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
  background-repeat: no-repeat;
  background-position: 50% 50%;

  animation: 2s linear 0s infinite alternate shining;
}

@keyframes shining {
  from {
    background-size: 75% 75%;
  }
  to {
    background-size: 100% 100%;
  }
}

.sun, .ring, .planet {
  position: absolute;
}

.ring {
  top: 50%;
  left: 50%;

  transform: translate(-50%, -50%);
}

.sun {
  width: 512px;
  height: 512px;

  top: 50%;
  left: 50%;

  background-image: url('@/static/sun.png');

  animation: 25s linear 0s infinite rotating;
}

@keyframes rotating {
  from {
    transform: translate(-50%, -50%) rotate(0deg);
  }
  to {
    transform: translate(-50%, -50%) rotate(360deg);
  }
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

.planet {
  width: 102px;
  height: 102px;

  transition: 0.1s;

  &:hover {
    width: 107px;
    height: 107px;

    margin-top: -2.5px;
    margin-left: -2.5px;
  }
}

.mercury {
  top: 1169px;
  left: 1319px;
}

.venus {
  top: 537px;
  left: 1133px;
}

.earth {
  top: 879px;
  left: 1542px;
}

.mars {
  top: 553px;
  left: 1486px;
}

.jupiter {
  top: 307px;
  left: 1310px;
}

.saturn {
  top: 1426px;
  left: 1690px;
}

.uranus {
  top: 1091px;
  left: 1904px;
}

.neptune {
  top: 683px;
  left: 1960px;
}
</style>
