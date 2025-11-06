<template>
  <div class="purple-background full-height">
    <div class="page-content-container">
      <h1>Pricing and Services</h1>
      <div class="pricing-container">
        <div class="pricing-box rounded">
          <p>This is an example text box with rounded edges. It contains pricing information and service details.</p>
        </div>
        <div class="pricing-box">
          <p>This is another example text box. It displays additional information about services and pricing options.
          </p>
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
  padding: 1.5rem;
  background-color: #f5f5f5;
  border: 1px solid #e0e0e0;
}

.pricing-box.rounded {
  border-radius: 12px;
}
</style>