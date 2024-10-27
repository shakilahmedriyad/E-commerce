<script setup lang="ts">
import { Link } from "@inertiajs/vue3";
import HeartIcons from "@/Icons/Heart-icons.vue";
import CartIcons from "@/Icons/Cart-icons.vue";
import Searchbar from "@/Components/ui/searchbar.vue";

const NavItem = [
    { label: "Home", slug: "/" },
    { label: "Contact", slug: "/contact" },
    { label: "About", slug: "/about" },
];
</script>
<template>
    <nav class="border-b">
        <content
            class="max-w-[80rem] w-full flex items-center justify-between py-5 mx-auto"
        >
            <Link href="/">
                <h1 class="text-3xl cursor-pointer font-bold">Exclusive</h1>
            </Link>

            <ul class="flex gap-5">
                <Link
                    :href="item.slug"
                    class="cursor-pointer"
                    v-for="item in NavItem"
                    :key="item.label"
                >
                    <li>
                        {{ item.label }}
                    </li>
                </Link>
            </ul>
            <div class="flex items-center">
                <Searchbar />
                <div
                    class="p-2 ml-2 rounded-full hover:bg-gray-200 cursor-pointer flex justify-center items-center"
                >
                    <HeartIcons class="w-[1.5rem]" />
                </div>
                <div
                    class="p-2 rounded-full hover:bg-gray-200 cursor-pointer flex justify-center items-center"
                >
                    <CartIcons class="w-[1.6rem]" />
                </div>
            </div>
        </content>
    </nav>
</template>
