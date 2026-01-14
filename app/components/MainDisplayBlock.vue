<template>
  <div class="main-display-block">
    <slot />
  </div>
</template>

<style scoped>
.main-display-block {
  width: 100%;
  min-height: calc(100vh / 3);
  margin: 0 auto;
  display: flex;
  align-items: center;
  justify-content: center;
}
.main-display-block:nth-child(odd) {
  background-color: #c1bad9;
}
.main-display-block:nth-child(even) {
  background-color: #ebd0a0;
}

/* On mobile, allow blocks to grow to fit content */
@media (max-width: 768px) {
  .main-display-block {
    height: auto;
    min-height: auto;
    padding: 2rem 1rem;
  }
}
</style>