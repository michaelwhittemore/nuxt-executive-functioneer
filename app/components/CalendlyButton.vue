<template>
    <div class="calendly-button">
        <a href="https://calendly.com/mikah-mccabe/free-intro-call" target="_blank">
            <b>Click here to schedule a free intro call</b></a>
    </div>
</template>

<style scoped>
.calendly-button {
    margin: 2rem 0;
    text-align: center;
}

.calendly-button a {
    display: inline-block;
    background-color: #d1f0ee;
    color: #1f2937;
    text-decoration: underline;
    padding: 1rem 2rem;
    border: 1px solid black;
    border-radius: 12px;
    font-weight: 500;
    transition: all 0.2s;
}

.calendly-button a:hover {
    background-color: #b8e6e3;
    transform: translateY(-2px);
    box-shadow: 0 4px 8px rgba(0, 0, 0, 0.2);
}
</style>