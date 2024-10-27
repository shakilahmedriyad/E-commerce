<script setup lang="ts">
import NavBar from "@/Components/NavBar/NavBar.vue";
</script>
<template>
    <main>
        <NavBar />
        <section class="max-w-[80rem] mx-auto">
            <slot />
        </section>
    </main>
</template>
