<template>
  <div class="main-display-container">
    <MainDisplayBlock>
      <h1>Empower Your Brain</h1>
    </MainDisplayBlock>
    <MainDisplayBlock>
      <h1>Block Two</h1>
    </MainDisplayBlock>
    <MainDisplayBlock>
      <div class="about-content">
        <p>About Me</p>
        <img src="/img/mikah2.jpeg" alt="Mikah Headshot" />
      </div>
    </MainDisplayBlock>
  </div>
</template>

<style scoped>
.about-content {
  width: 100%;
  height: 100%;
  display: flex;
  flex-direction: column;
  align-items: center;
  justify-content: center;
}

.about-content img {
  max-width: 100%;
  max-height: calc(100vh / 3 * 0.7);
  width: auto;
  height: auto;
  object-fit: contain;
  border: 2px solid black;
  border-radius: 12px;
}
</style>
