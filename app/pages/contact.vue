<template>
  <div class="purple-background full-height">
    <div class="page-content-container">
      <h1>Schedule a Free Meeting</h1>
      <div class="contact-container">
        <p>You'll get a Google Meet link, video optional. The intro meeting will take about 10 minutes, and you don't
          need to prepare anything in advance. If someone referred you to me, add their name to the form so they can
          earn a discount! </p>

        <p>Still not sure? I recommend reading the <NuxtLink to="/FAQs">FAQs</NuxtLink>.</p>
        <CalendlyButton />


      </div>

    </div>

    <div class="page-content-container">
      <h1>Returning Customers</h1>
      <div class="contact-container">
        <p>Worked with me before? Schedule a return session here!</p>
        <div class="contact-container">
          <CalendlyButton clientType="existing" />
        </div>
      </div>


    </div>

    <div class="page-content-container">
      <p>Any other questions? <b>
          <a href="mailto:mikah.mccabe@gmail.com?subject=About%20Your%20Decluttering%20Business">Email Me
          </a>
        </b>
        (mikah.mccabe@gmail.com)
      </p>

    </div>

  </div>

</template>
<style scoped>
.contact-container {
  padding-top: 1rem;
}
</style>
