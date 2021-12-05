<template>
  <a href="#start" v-scroll-to="{
    el: '#start',
    offset: -51
  }">
    <button>
      <div class="constellation" id="constellation-1"></div>
      Start
      <div class="constellation" id="constellation-2"></div>
    </button>
  </a>
</template>

<style lang="scss" scoped>
button {
  position: relative;

  width: 261px;
  height: 104px;

  margin-top: 136px;

  background: linear-gradient(93.82deg, #3342AE 53.7%, #314DC9 71.4%);
  border: 3px solid #fff;
  border-radius: 7px;

  color: #fff;
  font-size: 58px;
  font-weight: 200;

  transition: 0.3s;
  backface-visibility: hidden;

  &:hover {
    border: 5px solid #fff;
    cursor: pointer;
  }
}

a {
  color: white;
  text-decoration: none;
}

.constellation {
  position: absolute;

  width: 102px;
  height: 102px;

  background-size: cover;
}

#constellation-1 {
  top: -40px;
  left: -48px;

  background-image: url('@/static/stars/constellation-1.png');
}

#constellation-2 {
  top: 53px;
  right: -41px;

  background-image: url('@/static/stars/constellation-2.png');
}
</style>
