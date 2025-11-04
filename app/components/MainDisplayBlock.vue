<template>
  <div class="main-display-block">
    <slot />
  </div>
</template>

<style scoped>
.main-display-block {
  width: 100%;
  height: calc(100vh / 3);
  margin: 0 auto;
  display: flex;
  align-items: center;
  justify-content: center;
  overflow: hidden;
}
.main-display-block:nth-child(odd) {
  background-color: #c1bad9;
}
.main-display-block:nth-child(even) {
  background-color: #ebd0a0;
}
</style>