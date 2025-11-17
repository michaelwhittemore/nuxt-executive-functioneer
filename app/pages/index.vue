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
        <h1>Welcome</h1>
        <img src="/img/corgi.png" alt="Corgi" />
        <p>Do you have trouble focusing on tasks? Need an accountability buddy? Can't get a new habit to stick? I can help.</p>
        <!-- <img src="/img/happyDog.png" alt="Happy Dog" /> -->
      </div>
    </MainDisplayBlock>
    <MainDisplayBlock>
      <div class="constrained-content about-content">
        <img src="/img/mikah.jpeg" alt="Mikah Headshot" />
        <div class="about-content-text">
          <h2>About Me</h2>
          <p>Hello I'm Mikah! (she/her). I started a decluttering business, and quickly realized that the main thing my
            clients had in common was weapons-grade ADHD. I started reading, researching, and asking my ADHD-afflicted
            friends questions to learn everything I could. My background is in project management, where I spend a lot
            of time learning what's blocking someone from finishing a task and working with them to get past that block.
            I live with my husband, two cats, and a snake. I enjoy reading, listening to power metal, and avoiding going
            on hikes. </p>
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

/* Mobile responsive styles */
@media (max-width: 768px) {
  .constrained-content {
    height: auto;
    min-height: auto;
    padding: 1.5rem 1rem;
  }

  .brain-content img {
    max-height: 40vh;
    margin-bottom: 1rem;
  }

  .about-content {
    flex-direction: column;
    gap: 1.5rem;
  }

  .about-content img {
    max-width: 100%;
    max-height: 50vh;
    width: auto;
    margin: 0 auto;
  }

  .about-content-text {
    text-align: center;
  }

  .brain-content h1,
  .about-content-text h2 {
    font-size: 1.5rem;
    margin-bottom: 1rem;
  }

  .brain-content p,
  .about-content-text p {
    font-size: 0.9rem;
    line-height: 1.6;
  }
}
</style>
