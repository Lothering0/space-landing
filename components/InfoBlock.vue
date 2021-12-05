<template>
  <div
    class="info-block"
    :style="{ marginTop: marginTop + 'px' }"
    v-scroll-reveal="scrollRevealConfig"
  >
    <slot name="h1"></slot>
    <slot name="p"></slot>
  </div>
</template>

<script>
export default {
  data: () => ({
    scrollRevealConfig: {
      duration: 1000
    }
  }),
  props: {
    marginTop: String
  }
}
</script>

<style lang="scss" scoped>
.info-block {
  position: relative;
  width: 734px;

  margin: 0 auto;

  z-index: 2;
}

h1 {
  margin-bottom: 25px;
}

p {
  padding: 1px;

  font-size: 38px;
  font-weight: 300;
}

i {
  font-weight: 200;
  font-style: italic;
}
</style>
