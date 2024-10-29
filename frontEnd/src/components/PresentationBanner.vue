<template>
    <div class="banner">
        <div class="banner-header">
            <div class="profile-image"></div>
            <div class="headline">
                <h1>Turning Ideas into Digital Reality</h1>
            </div>
        </div>
        <div class="banner-body">
            <div>
                <h2>Hi, I'm Arthur Correa, a creative web developer from Cuiabá.</h2>
            </div>
            <div>
                <p>I design and build high-performance websites and systems that transform user experience and deliver
                    real results.</p>
            </div>
            <div class="call-to-action">
                <RouterLink to="/contact">
                    <button type="button" class="color-lunar-eclipse">Let's Collaborate</button>
                </RouterLink>
                <RouterLink to="/projects">
                    <button type="button" class="color-solar-eclipse">Explore My Work</button>
                </RouterLink>
            </div>
        </div>
        <div class="social-links">
            <button type="button" class="icon color-solar-eclipse">
                <font-awesome-icon :icon="['fab', 'instagram']" />
            </button>
            <button type="button" class="icon color-solar-eclipse">
                <font-awesome-icon :icon="['fab', 'square-facebook']" />
            </button>
            <button type="button" class="icon color-solar-eclipse">
                <font-awesome-icon :icon="['fab', 'linkedin-in']" />
            </button>
        </div>
    </div>
</template>

<script setup></script>

<style scoped>
.banner {
    @apply flex w-full h-96 bg-gradient-to-b delay-700;
    @apply bg-white;
}

.profile-image {
    @apply size-10 bg-cover bg-center rounded-full;
    background-image: url("/image/image-profile.jpg");
}

.banner-header {
    @apply flex flex-col justify-center items-start gap-4 h-full px-20;
}

.banner-body {
    @apply flex flex-col justify-center items-start gap-2 w-1/2 h-full px-20;
}

.headline {
    @apply flex;
}

.call-to-action {
    @apply flex gap-4 mt-8;
}

.social-links {
    @apply flex flex-col gap-2 p-6;
}

h1 {
    @apply text-5xl font-bold;
}

h2 {
    @apply text-3xl font-semibold;
}

p {
    @apply text-sm font-light;
}

button.color-lunar-eclipse {
    @apply bg-black text-white border-black;
    @apply hover:bg-white hover:text-black border-black;
}

button.color-solar-eclipse {
    @apply bg-white text-black border-black;
    @apply hover:bg-black hover:text-white border-black;
}

button.icon {
    @apply text-lg rounded-full;
}
</style>
