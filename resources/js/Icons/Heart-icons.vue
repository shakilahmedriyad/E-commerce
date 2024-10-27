<script setup lang="ts">
defineProps({
    class: String,
    fill: {
        type: String,
        default: "none",
    },
});
</script>
<template>
    <svg
        xmlns="http://www.w3.org/2000/svg"
        :class="class"
        viewBox="0 0 26 24"
        fill="none"
    >
        <path
            stroke-width="2"
            stroke="currentColor"
            d="m13 22.583-1.112-1.115-.021-.022-.023-.02c-3.397-3.015-6.126-5.47-8.015-7.777C1.95 11.356 1 9.326 1 7.174 1 3.68 3.675 1 7.15 1c1.91 0 3.842.91 5.086 2.384L13 4.29l.764-.906C15.008 1.909 16.94 1 18.85 1 22.325 1 25 3.68 25 7.174c0 2.152-.95 4.182-2.829 6.475-1.89 2.307-4.618 4.762-8.015 7.777l-.023.02-.021.022L13 22.583Z"
        />
    </svg>
</template>
