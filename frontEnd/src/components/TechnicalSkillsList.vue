<template>
    <section class="skills-section">
        <h2 class="skills-title">Habilidades Técnicas</h2>

        <!-- Carrossel do Swiper -->
        <swiper :slides-per-view="3" space-between="30" navigation pagination loop>
            <swiper-slide v-for="(category, index) in skills" :key="index" class="swiper-slide">
                <div class="skill-category">
                    <h3 class="category-title">{{ category.title }}</h3>
                    <ul class="skill-list">
                        <li v-for="(skill, idx) in category.items" :key="idx" class="skill-item">
                            <span>{{ skill.name }}</span>
                            <span :class="['skill-level', skill.level]">{{ skill.displayLevel }}</span>
                        </li>
                    </ul>
                </div>
            </swiper-slide>
        </swiper>
    </section>
</template>

<script>
import { Swiper, SwiperSlide } from 'swiper/vue';
import 'swiper/swiper-bundle.css';

export default {
    components: {
        Swiper,
        SwiperSlide,
    },
    data() {
        return {
            skills: [
                {
                    title: "Linguagens de Programação",
                    items: [
                        { name: "JavaScript", level: "advanced", displayLevel: "Avançado" },
                        { name: "Python", level: "intermediate", displayLevel: "Intermediário" },
                        { name: "PHP", level: "intermediate", displayLevel: "Intermediário" },
                    ],
                },
                {
                    title: "Frameworks & Bibliotecas",
                    items: [
                        { name: "Vue.js", level: "advanced", displayLevel: "Avançado" },
                        { name: "React.js", level: "intermediate", displayLevel: "Intermediário" },
                        { name: "Node.js", level: "advanced", displayLevel: "Avançado" },
                    ],
                },
                {
                    title: "Ferramentas & Tecnologias",
                    items: [
                        { name: "Docker", level: "intermediate", displayLevel: "Intermediário" },
                        { name: "Git", level: "advanced", displayLevel: "Avançado" },
                        { name: "PostgreSQL", level: "intermediate", displayLevel: "Intermediário" },
                    ],
                },
            ],
        };
    },
};
</script>

<style scoped>
.skills-section {
    @apply py-16 bg-gray-100;
}

.skills-title {
    @apply text-4xl font-bold text-center text-blue-800 mb-8;
}

.skill-category {
    @apply bg-white shadow-lg rounded-lg p-6;
}

.category-title {
    @apply text-2xl font-semibold text-blue-800 mb-4;
}

.skill-list {
    @apply space-y-2;
}

.skill-item {
    @apply flex justify-between;
}

.skill-level {
    @apply font-bold;
}

.advanced {
    @apply text-green-500;
}

.intermediate {
    @apply text-yellow-500;
}

.swiper-slide {
    @apply flex justify-center;
}
</style>