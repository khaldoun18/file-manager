<template>
    <div class="flex w-full h-screen gap-4 bg-gray-50">
        <Navigation></Navigation>

        <main class="flex flex-col flex-1 px-4 overflow-hidden">
            <div class="flex items-center justify-between w-full">
                <SearchForm></SearchForm>
                <UserSettingsDropdown></UserSettingsDropdown>
            </div>
            <div class="flex flex-col flex-1 overflow-hidden">
                <slot></slot>
            </div>
        </main>
    </div>
</template>


<script setup>
import Navigation from '@/Components/app/Navigation.vue';
import SearchForm from '@/Components/app/SearchForm.vue';
import UserSettingsDropdown from '@/Components/app/UserSettingsDropdown.vue';






</script>
