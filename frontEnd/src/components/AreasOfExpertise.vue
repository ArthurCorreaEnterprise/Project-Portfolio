<template>
    <div class="style-00">
        <div>
            <h1>Areas of Expertise</h1>
        </div>
        <div>
            <div>
                <font-awesome-icon :icon="['fab', 'square-facebook']" />
                <h2>Ux & Ui</h2>
                <p>Designing interfaces that are intuitive, efficient, and enjoyable to use</p>
            </div>
            <div>
                <font-awesome-icon :icon="['fab', 'square-facebook']" />
                <h2>Web & Mobile App</h2>
                <p>Transforming ideas into exceptional web and mobile app experiences</p>
            </div>
            <div>
                <font-awesome-icon :icon="['fab', 'square-facebook']" />
                <h2>Design & Creative</h2>
                <p>crafting visually stunning designs that connect whit your audiences</p>
            </div>
            <div>
                <font-awesome-icon :icon="['fab', 'square-facebook']" />
                <h2>Development</h2>
                <p>bringing your vision to life with the lasted techonology and design trends</p>
            </div>
        </div>
    </div>
</template>

<script setup>

</script>

<style scoped>
.style-00 {
    @apply flex flex-col justify-center items-center w-full h-full p-8 ;
    @apply bg-gray-100;
}
</style>