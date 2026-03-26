<template>
    <div class="yellow-background full-height">
        <div class="page-content-container">
            <h1>Testimonials</h1>
            <p>Click the arrows below to scroll through testimonials.</p>
            <ClientOnly>
                <div
                    class="senja-embed"
                    data-id="bcf7164b-35a2-4b97-8f00-cf44518d85d1"
                    data-mode="shadow"
                    data-lazyload="false"
                ></div>
            </ClientOnly>
        </div>
    </div>
</template>

<script setup>
onMounted(() => {
    const existingScript = document.getElementById("senja-widget-script")
    if (existingScript) return

    const script = document.createElement("script")
    script.id = "senja-widget-script"
    script.src = "https://widget.senja.io/widget/bcf7164b-35a2-4b97-8f00-cf44518d85d1/platform.js"
    script.type = "text/javascript"
    script.async = true
    document.body.appendChild(script)
})
</script>

<style scoped>
.testimonial-container {
    display: flex;
    flex-direction: column;
    gap: 2rem;
    margin-top: 2rem;
}

.testimonial-box {
    flex: 1;
    border: 1px solid black;
    background-color: #c1bad9;
    padding: 1.5rem;
}

.testimonial-box.rounded {
    border-radius: 12px;
}

.senja-embed {
    display: block;
    width: 100%;
    min-height: 320px;
}
</style>