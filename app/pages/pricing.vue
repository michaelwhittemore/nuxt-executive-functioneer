<script setup>
</script>

<template>
  <div class="purple-background full-height">
    <div class="page-content-container">
      <h1>Pricing and Services</h1>
      <br></br> <!-- add a line break, probably format this better -->
      <h3>How much do you cost?</h3>
      <p>In-person decluttering sessions cost <b>$50 per hour </b>with a 2-hour minimum. I also offer carting off a load
        of
        items to a donation center for a $25 flat fee per trip.</p> <br></br>
      <h3>Where do you operate?</h3>
      <p>I can travel to any home in the San Francisco Bay Area.
      </p>
      <div class="pricing-container">
        <div class="pricing-box rounded yellow-pricing-box">
          <div class="centered-text-header"> Menu of Services</div>
          <p>During a session, I can help you with:</p>
          <ul class="pricing-list">
            <li>Sorting piles of stuff and helping you make decisions about each object</li>
            <li>Body doubling (observing you until you complete a task)</li>
            <li>Replying to difficult emails or texts</li>
            <li>Advice on forming a new habit (e.g. exercising, eating breakfast, flossing)</li>
            <li>Decreasing negative self-talk</li>
            <li>Accountability and follow-up on important tasks</li>
            <li>Booking or preparing for a trip</li>
            <li>Prioritizing personal or business tasks</li>
          </ul>
          <br />
          <p><b>Please note - </b> for liability purposes, I cannot assist with tasks that expose me to:</p>
            <ul class="pricing-list">
              <li>Proprietary data or sensitive financial information</li>
              <li>Biohazards such as loose sharps, active bedbug/flea/scabies infestations, bodily fluids</li>
              <li>Active crisis situations requiring medical or psychiatric intervention</li>

            </ul>
        </div>

      </div>
      <CalendlyButton />
    </div>
  </div>
</template>

<style scoped>
.pricing-list {
  list-style-position: inside
}

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