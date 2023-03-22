<script setup>
import AuthenticatedLayout from "@/Layouts/AuthenticatedLayout.vue";
import UpdateProfileForm from "./Components/Profile.vue";
import UpdateEduBackgroundForm from "./Components/EduBackground.vue";
import UpdateAddressForm from "./Components/Address.vue";
import { Head } from "@inertiajs/vue3";

// defineProps({
//     mustVerifyEmail: Boolean,
//     status: String,
// });
</script>

<template>
    <Head title="Sample" />

    <AuthenticatedLayout>
        <template #header>
            <h2
                class="font-semibold text-xl text-gray-800 dark:text-gray-200 leading-tight"
            >
                Task
            </h2>
        </template>

        <div class="py-12">
            <div class="max-w-7xl mx-auto sm:px-6 lg:px-8 space-y-6">
                <div
                    class="p-4 sm:p-8 bg-white dark:bg-gray-800 shadow sm:rounded-lg"
                >
                    <UpdateProfileForm class="max-w-xl" />
                </div>

                <div class="p-4 sm:p-8 dark:bg-gray-800 shadow sm:rounded-lg">
                    <UpdateAddressForm class="max-w-xl" />
                </div>

                <div
                    class="p-4 sm:p-8 bg-white dark:bg-gray-800 shadow sm:rounded-lg"
                >
                    <UpdateEduBackgroundForm class="max-w-xl" />
                </div>
            </div>
        </div>
    </AuthenticatedLayout>
</template>
