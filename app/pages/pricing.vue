<script setup>
import { onMounted } from 'vue';
onMounted(() => {
  const script = document.createElement('script');
  script.src = 'https://assets.calendly.com/assets/external/widget.js';
  script.async = true;
  document.body.appendChild(script);
});
</script>

<template>
  <div class="purple-background full-height">
    <div class="page-content-container">
      <h1>Pricing and Services</h1>
      <br></br> <!-- add a line break, probably format this better -->
      <h3>How much do you cost?</h3>
      <p>Phi universal law constant occurrence
        design absent of flaws natural appearance
        with DNA and galaxies we approach infinity
        nothing split by unity is the constant creation
        divine proportion defines perfection
        with this comes enticing shapes
        supreme equation from formation
        the formula of 1.618
        a pattern beyond man a blueprint of divinity
        the spiral of god eternal plan forever the line divided
        nothing split by unity is the constant creation
        divine proportion defines perfection
        with this comes enticing shapes
        supreme equation from formation
        the formula of 1.618
        phi patterns symmetry surrounds us
        design precise product of the universe
        with DNA and galaxies we are one with infinity</p>
      <div class="pricing-container">
        <div class="pricing-box rounded yellow-pricing-box">
          <div class="centered-text-header"> Menu of Services</div>
          <ul>
            <li> Item one</li>
            <li> Item two</li>
            <li> Item three</li>
          </ul>
        </div>
        <!-- <iframe src="https://calendly.com/mikah-mccabe/free-intro-call" style="width: 100%; min-width: 320px; height: 700px;"
            frameborder="0"></iframe> -->
        <!-- <div class="calendly-inline-widget" data-url="https://calendly.com/mikah-mccabe/free-intro-call"
            style="width:90%;height:400px;"></div> -->
        <div class="calendly-inline-widget pricing-box"
        data-url="https://calendly.com/mikah-mccabe/free-intro-call">

        </div>
      </div>
    </div>
  </div>
</template>

<style scoped>
.pricing-container {
  display: flex;
  gap: 2rem;
  margin-top: 2rem;
}

.pricing-box {
  flex: 1;
  border: 1px solid black;
  min-height: 400px;
}

.yellow-pricing-box {
  background-color: #ebd0a0;
  padding: 1.5rem;
}

.pricing-box.rounded {
  border-radius: 12px;
}

.centered-text-header {
  text-align: center;
  font-weight: bold;
  font-size: 1.25rem;
}
</style>