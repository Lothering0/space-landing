<template>
  <div>
    <div class="block">
      <div class="header">
        <h1>Explore the space</h1>
        <Button />
      </div>
    </div>

    <Container />
  </div>
</template>

<style lang="scss" scoped>
.block {
  width: 100%;
  height: 900px;
  background-image: url('@/static/space-background.jpg');
  background-size: 100%;
  background-repeat: no-repeat;

  .header {
    display: flex;
    flex-direction: column;
    align-items: center;

    position: sticky;
    top: 0;

    width: fit-content;

    padding-top: 196px;
    padding-left: 172px;
    padding-bottom: 55px;
  }
}
</style>
