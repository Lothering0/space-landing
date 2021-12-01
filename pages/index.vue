<template>
  <div>
    <div class="block">
      <div class="header">
        <h1>Explore the space</h1>
        <button>Start</button>
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
  }
}

button {
  width: 261px;
  height: 104px;

  margin-top: 136px;

  background: transparent;
  border: 3px solid #fff;
  border-radius: 7px;

  color: #fff;
  font-size: 58px;
  font-weight: 200;

  transition: 0.6s;

  &:hover {
    background: #fff;
    color: #403c63;
    cursor: pointer;
  }
}
</style>
