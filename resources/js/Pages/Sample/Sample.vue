<script setup>
import AuthenticatedLayout from '@/Layouts/AuthenticatedLayout.vue';
// import UpdateProfileForm from './Partials/Profile.vue';
// import UpdateEduBackgroundForm from './Partials/EduBackground.vue';
// import UpdateAddressForm from './Partials/Address.vue';
import { Head } from '@inertiajs/vue3';

// defineProps({
//     mustVerifyEmail: Boolean,
//     status: String,
// });
</script>

<template>
    <Head title="Sample" />

    <AuthenticatedLayout>
        <template #header>
            <h2 class="font-semibold text-xl text-gray-800 dark:text-gray-200 leading-tight">Task</h2>
        </template>

        <div class="py-12">
            <div class="max-w-7xl mx-auto sm:px-6 lg:px-8 space-y-6">
                <div class="p-4 sm:p-8 bg-white dark:bg-gray-800 shadow sm:rounded-lg">
                    <!-- <UpdateProfileInformationForm
                        :must-verify-email="mustVerifyEmail"
                        :status="status"
                        class="max-w-xl"
                    /> -->
                </div>

                <div class="p-4 sm:p-8 dark:bg-gray-800 shadow sm:rounded-lg">
                    <h1 class="block text-white text-lg font-bold">EDUCATION</h1>
                    <form class="shadow-md rounded px-8 pt-6 pb-8 mb-4">
                        <div class="mb-4">
                        <label class="block text-white text-sm font-bold mb-2" for="fos">
                            Field of study
                        </label>
                        <input class="shadow appearance-none border rounded w-full py-2 px-3 text-gray-700 leading-tight focus:outline-none focus:shadow-outline" id="fos" type="text" placeholder="Field of Study">
                        </div>
                        <div class="mb-6">
                        <label class="block text-white text-sm font-bold mb-2" for="cgpa">
                            CGPA
                        </label>
                        <input class="shadow appearance-none border border-red-500 rounded w-full py-2 px-3 text-gray-700 mb-3 leading-tight focus:outline-none focus:shadow-outline" id="cgpa" type="text" placeholder="CGPA">
                        </div>

                        <button class="bg-blue-500 hover:bg-blue-700 text-white font-bold py-2 px-4 rounded-full">
                        Save
                        </button>
                    </form>
                </div>

                <div class="p-4 sm:p-8 bg-white dark:bg-gray-800 shadow sm:rounded-lg">
                    <!-- <DeleteUserForm class="max-w-xl" /> -->
                </div>
            </div>
        </div>
    </AuthenticatedLayout>
</template>
