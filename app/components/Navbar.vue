<template>
    <nav class="navbar" :class="{ collapsed: isCollapsed }">
        <button class="toggle-button" @click="toggleSidebar" :aria-label="isCollapsed ? 'Expand sidebar' : 'Collapse sidebar'">
            <span class="hamburger-icon">
                <!-- Built out of three line-spans to make a hamburger icon -->
                <span></span>
                <span></span>
                <span></span>
            </span>
        </button>
        <div class="navbar-container">
            <NuxtLink to="/" class="navbar-link">
                <span class="link-text">Home</span>
            </NuxtLink>
            <NuxtLink to="/pricing" class="navbar-link">
                <span class="link-text">Pricing and Services</span>
            </NuxtLink>
            <NuxtLink to="/FAQs" class="navbar-link">
                <span class="link-text">FAQs</span>
            </NuxtLink>
            <NuxtLink to="/contact" class="navbar-link">
                <span class="link-text">Contact</span>
            </NuxtLink>
        </div>
    </nav>
</template>

<script setup>
import { ref } from 'vue'

const device = useDevice()

// Use device detection from @nuxtjs/device which works with SSR
// Collapse on mobile/tablet, expand on desktop
const isCollapsed = ref(device.isMobile || device.isTablet)

const toggleSidebar = () => {
    isCollapsed.value = !isCollapsed.value
}
</script>

<style scoped>
.navbar {
    /* Lock width by setting width, min-width, and max-width to the same value.
       This prevents the flex container from resizing the navbar based on content or available space. */
    width: 200px;
    min-width: 200px;
    max-width: 200px;
    min-height: 100vh;
    background-color: #a7d9d6;
    border-right: 1px solid black;
    transition: width 0.3s ease, min-width 0.3s ease, max-width 0.3s ease;
    position: relative;
    overflow: hidden;
    flex-shrink: 0;
    flex-grow: 0;
}

.navbar.collapsed {
    width: 60px;
    min-width: 60px;
    max-width: 60px;
}

.toggle-button {
    position: absolute;
    top: 1rem;
    left: 0.5rem;
    background: transparent;
    border: none;
    cursor: pointer;
    padding: 0.5rem;
    z-index: 10;
    display: flex;
    align-items: center;
    justify-content: center;
    border-radius: 4px;
    transition: background-color 0.2s;
}

.toggle-button:hover {
    background-color: rgba(0, 0, 0, 0.1);
}

.hamburger-icon {
    display: flex;
    flex-direction: column;
    gap: 4px;
    width: 20px;
}

.hamburger-icon span {
    display: block;
    height: 2px;
    width: 100%;
    background-color: #1f2937;
    border-radius: 2px;
}

.navbar-container {
    display: flex;
    flex-direction: column;
    padding: 1rem;
    gap: 0.75rem;
    padding-top: 3.5rem;
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
    text-align: center;
    word-wrap: break-word;
}

.navbar.collapsed .navbar-link {
    display: none;
}

.link-text {
    display: inline-block;
    opacity: 1;
    transition: opacity 0.2s;
}

.navbar.collapsed .link-text {
    opacity: 0;
    width: 0;
    overflow: hidden;
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
