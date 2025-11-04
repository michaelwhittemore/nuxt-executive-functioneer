// The default layout is the main layout for the entire application. 
// It includes the navbar, the footer, and the slot for the content.
<template>
    <div class="app-container">
        <Navbar />
        <div class="content-container">
            <slot />
        </div>
        <!-- <Footer /> -->
    </div>
</template>
<style>
.app-container {
    display: flex;
    min-height: 100vh;
}

.content-container {
    flex: 1;
    padding: 0;
    width: 100%;
}
</style>