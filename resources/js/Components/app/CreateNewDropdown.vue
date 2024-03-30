<template>
    <Menu as="div" class="relative inline-block text-left">

        <MenuButton
            class="flex justify-center w-full gap-x-1.5 rounded-md bg-white px-3 py-2 text-sm font-semibold text-gray-900 shadow-sm ring-1 ring-inset ring-gray-300 hover:bg-gray-50">
            <a href=""> Create New</a>

        </MenuButton>

        <transition enter-active-class="transition duration-100 ease-out"
            enter-from-class="transform scale-95 opacity-0" enter-to-class="transform scale-100 opacity-100"
            leave-active-class="transition duration-75 ease-in" leave-from-class="transform scale-100 opacity-100"
            leave-to-class="transform scale-95 opacity-0">
            <MenuItems
                class="absolute left-0 w-32 mt-2 origin-top-right bg-white divide-y divide-gray-100 rounded-md shadow-lg ring-1 ring-black/5 focus:outline-none">
                <div class="px-1 py-1">
                    <MenuItem v-slot="{ active }">

                    <a class="block px-4 py-2 text-sm text-gray-700" href=""> New Folder</a>

                    </MenuItem>

                </div>

                <div class="px-1 py-1">
                    <MenuItem v-slot="{ active }">

                    <a class="block px-4 py-2 text-sm text-gray-700" href=""> Upload Folder</a>

                    </MenuItem>

                    <MenuItem v-slot="{ active }">

                    <a class="block px-4 py-2 text-sm text-gray-700" href="">Upload File</a>


                    </MenuItem>

                </div>

            </MenuItems>
        </transition>
    </Menu>

</template>

<script setup>
import { Menu, MenuButton, MenuItem, MenuItems } from '@headlessui/vue';


</script>
