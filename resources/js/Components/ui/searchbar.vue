<script setup lang="ts">
import GlassIcons from "@/Icons/Glass-icons.vue";
</script>

<template>
    <div class="flex border bg-[F5F5F5] rounded-md items-center px-2">
        <input
            type="text"
            class="py-2 bg-[F5F5F5] focus:outline-none px-2 text-sm"
            placeholder="What are you looking for?"
        />
        <GlassIcons class="w-5" />
        <div></div>
    </div>
</template>
