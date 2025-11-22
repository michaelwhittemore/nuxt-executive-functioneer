<script setup>
</script>

<template>
  <div class="purple-background full-height">
    <div class="page-content-container">
      <h1>Pricing and Services</h1>
      <br></br> <!-- add a line break, probably format this better -->
      <h3>How much do you cost?</h3>
      <p>I charge a flat $50 rate <b>per session</b>, due at the end of a given session. A coaching session is defined as an
        online video in which I provide gentle, compassionate encouragement and accountability to achieve one or more of
        the menu items below.</p> <br></br>
      <p>If you're currently in the San Francisco Bay area, ask me about in-person sessions! These cost $50 <b>per hour</b> and
        allow me to act as a specialized organizer for physical items or per-hour rentable body double.</p>
      <div class="pricing-container">
        <div class="pricing-box rounded yellow-pricing-box">
          <div class="centered-text-header"> Menu of Services</div>
          <p>During a session, I can assist with:</p>
          <ul class="pricing-list">
            <li> Replying to difficult emails or texts </li>
            <li> Forming a new habit (e.g. exercising, eating breakfast, flossing)</li>
            <li>Body doubling (observing you until you complete a task)</li>
            <li>Epic, personalized motivational speeches</li>
            <li>Decreasing negative self-talk</li>
            <li>Accountability and follow-up on important tasks</li>
            <li>Sorting piles of stuff and making decisions about each object</li>
            <li>Booking or preparing for a trip</li>
            <li>Decisionmaking</li>
            <li>Improving communication with co-workers</li>
          </ul>

          <p><b>Please note:</b> for liability purposes, I cannot assist with tasks that expose me to proprietary data
            or financial information.</p>
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