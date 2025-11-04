<template>
    <nav class="navbar">
        <div class="navbar-container">
            <NuxtLink to="/" class="navbar-link">Home</NuxtLink>
            <NuxtLink to="/pricing" class="navbar-link">Pricing</NuxtLink>
            <NuxtLink to="/FAQs" class="navbar-link">FAQs</NuxtLink>
            <NuxtLink to="/contact" class="navbar-link">Contact</NuxtLink>
        </div>
    </nav>
</template>

<style scoped>
.navbar {
    width: 200px;
    height: 100vh;
    background-color: #a7d9d6;
    border-right: 1px solid #e5e7eb;
}

.navbar-container {
    display: flex;
    flex-direction: column;
    padding: 1rem;
    gap: 0.75rem;
}

.navbar-link {
    color: #1f2937;
    text-decoration: none;
    font-weight: 500;
    transition: all 0.2s;
    padding: 0.75rem 1.25rem;
    background-color: #d1f0ee;
    border-radius: 999px;
    display: block;
}

.navbar-link:hover {
    color: #1f2937;
    background-color: #b8e6e3;
}

.navbar-link.router-link-active {
    color: #1f2937;
    background-color: #b8e6e3;
}
</style>
