<template>
  <main :style="{
    'transform': `scale(${width})`,
    left
  }">
    <Nuxt />
  </main>
</template>

<script>
export default {
  data: () => ({ windowWidth: window.innerWidth }),
  watch: {
    windowWidth() {
      return window.innerWidth
    }
  },
  computed: {
    width() {
      return this.windowWidth / 1600
    },
    left() {
      return (this.windowWidth - 1600) / 2 + 'px'
    }
  },
  methods: {
    onResize() {
      this.windowWidth = window.innerWidth
    }
  },
  mounted() {
    this.$nextTick(() => {
      window.addEventListener('resize', this.onResize)
    })
  },
  beforeDestroy() {
    window.removeEventListener('resize', this.onResize)
  },
}
</script>

<style lang="scss">
@import url('https://fonts.googleapis.com/css2?family=Poppins:ital,wght@0,200;0,300;0,600;0,700;1,200&display=swap');

html {
  overflow-x: hidden;
}

body {
  margin: 0;
  padding: 0;

  font-family: 'Poppins';
  color: #fff;
}

* {
  user-select: none;
  -ms-overflow-style: none;  /* IE and Edge */
  scrollbar-width: none;  /* Firefox */
}

*::-webkit-scrollbar {
  display: none; /* Chrome */
}

h1, p, ul {
  margin: 0;
  padding: 0;
}

li {
  list-style: none;
}

#__layout {
  position: relative;
  width: 0;
}

main {
  position: absolute;
  inset: 0;
  width: 1600px;
}

h1 {
  font-size: 68px;
  font-weight: 700;
  text-transform: uppercase;
}

.planet {
  background-size: cover;

  animation: 5s linear 0s alternate infinite rotating;
}

@keyframes rotating {
  from {
    transform: rotate(0deg);
  }
  to {
    transform: rotate(12deg);
  }
}

.mercury {
  background-image: url('@/static/planets/mercury.png');
}

.venus {
  background-image: url('@/static/planets/venus.png');
}

.earth {
  background-image: url('@/static/planets/earth.png');
}

.mars {
  background-image: url('@/static/planets/mars.png');
}

.jupiter {
  background-image: url('@/static/planets/jupiter.png');
}

.saturn {
  background-image: url('@/static/planets/saturn.png');
}

.uranus {
  background-image: url('@/static/planets/uranus.png');
}

.neptune {
  background-image: url('@/static/planets/neptune.png');
}
</style>
