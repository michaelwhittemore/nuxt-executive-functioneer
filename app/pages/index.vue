<template>
  <div class="main-display-container">
    <MainDisplayBlock>
      <div class="constrained-content brain-content">
        <h1>Empower Your Brain</h1>
        <img src="/img/brain.png" alt="Brain" />
      </div>
    </MainDisplayBlock>
    <MainDisplayBlock>
      <div class="constrained-content brain-content">
        <h1>Block Two</h1>
        <img src="/img/corgi.jpeg" alt="Corgi" />
      </div>
    </MainDisplayBlock>
    <MainDisplayBlock>
      <div class="constrained-content about-content">
        <img src="/img/mikah2.jpeg" alt="Mikah Headshot" />
        <div class="about-content-text">
          <p>About Me</p>
          <p>Excuse me, can you tell me the worst thing you've heard about me?
            Maybe that I'm a little harlot, homicidal queen
            You know I heard (heard) that I don't belong in this scene
            Sex metal Barbie, (whore), attention fiend
            (You know I) heard (heard) that I'm a hater's dream
            Low class, white trash, I'm so obscene
            (You know I) heard that I should be ashamed
            Still they hold their fists in the air, screaming my name
            Come on!</p>
        </div>

      </div>
    </MainDisplayBlock>
  </div>
</template>

<style scoped>
.constrained-content {
  width: 100%;
  height: 100%;
  display: flex;
  align-items: center;
  justify-content: center;
  padding: 2rem;
}

.brain-content {
  flex-direction: column;
}

.brain-content img {
  max-width: 100%;
  max-height: calc(100vh / 3 * 0.7);
  width: auto;
  height: auto;
  object-fit: contain;
}

.about-content {
  flex-direction: row;
  gap: 2rem;
}

.about-content img {
  max-width: 40%;
  max-height: calc(100vh / 3 * 0.8);
  width: auto;
  height: auto;
  object-fit: contain;
  border: 2px solid black;
  border-radius: 12px;
}

.about-content-text {
  flex: 1;
  display: flex;
  flex-direction: column;
  justify-content: center;
}
</style>
