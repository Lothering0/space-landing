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

body {
  margin: 0;
  padding: 0;

  font-family: 'Poppins';
  color: #fff;
}

* {
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
  text-transform: uppercase;
}
</style>
