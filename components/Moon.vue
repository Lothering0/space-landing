<template>
  <div class="moon" :style="{ top, left }">
    <div class="image"></div>
    <div class="name" :style="{ backgroundColor }">{{name}}</div>
  </div>
</template>

<script>
export default {
  props: {
    name: String,
    top: String,
    left: String,
    backgroundColor: String
  }
}
</script>

<style>
.moon {
  position: absolute;

  z-index: 2;
}

.image {
  width: 132px;
  height: 132px;

  margin: 0 auto;

  background-image: url('@/static/moon.png');
  background-size: cover;
}

.name {
  margin-top: 23px;

  border-radius: 5px;

  font-size: 35px;
  font-weight: 600;
  text-align: center;
}
</style>