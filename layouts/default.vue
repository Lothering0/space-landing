<template>
  <main :style="{
    'transform': `scale(${width})`,
    left
  }">
    <Nuxt />
  </main>
</template>

<script>
// (width - 1600) / 2
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

<style>
body {
  margin: 0;
  padding: 0;
  font-family: 'Ubuntu';
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
</style>
