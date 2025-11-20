<template>
  <div class="calendly-button">
    <a href="https://calendly.com/mikah-mccabe/free-intro-call" target="_blank"> 
    Click here to schedule a free intro call</a>
    </div>
</template>

<style scoped>
.calendly-button {
  margin: 2rem 0;
  text-align: center;
}

.calendly-button a {
  display: inline-block;
  background-color: #ebd0a0;
  color: #1f2937;
  text-decoration: none;
  padding: 1rem 2rem;
  border: 1px solid black;
  border-radius: 12px;
  font-weight: 500;
  transition: all 0.2s;
}

.calendly-button a:hover {
  background-color: #d4c08f;
  transform: translateY(-2px);
  box-shadow: 0 4px 8px rgba(0, 0, 0, 0.2);
}
</style>