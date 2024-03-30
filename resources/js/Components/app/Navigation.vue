<template>
    <nav class="min-w-[200px]">
        <div class="h-[80px] px-3 flex items-center gap-3">
            <Link href="">
            <ApplicationLogo class="block w-auto text-gray-800 fill-current h-9" />
            </Link>
            Laravel storage
        </div>
        <div class="px-3">
            <CreateNewDropdown></CreateNewDropdown>

            <div class="py-3">
                <NavLink href="">My files</NavLink>
                <NavLink href="">Shared with me</NavLink>
                <NavLink href="">Shared by me</NavLink>
                <NavLink href="">Trash</NavLink>

            </div>
        </div>
    </nav>
</template>

<script setup>
import { Link } from '@inertiajs/vue3'
import ApplicationLogo from '@/Components/ApplicationLogo.vue';
import CreateNewDropdown from './CreateNewDropdown.vue';
import NavLink from '../NavLink.vue';
</script>
