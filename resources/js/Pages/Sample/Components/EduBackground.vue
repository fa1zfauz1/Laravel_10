<template>
    <h1 class="block text-white text-lg font-bold">EDUCATION</h1>
    <form class="shadow-md rounded px-8 pt-6 pb-8 mb-4">
        <div class="mb-4">
            <label class="block text-white text-sm font-bold mb-2" for="fos">
                Field of study
            </label>
            <input
                class="shadow appearance-none border rounded w-full py-2 px-3 text-gray-700 leading-tight focus:outline-none focus:shadow-outline"
                id="fos"
                type="text"
                placeholder="Field of Study"
            />
        </div>
        <div class="mb-6">
            <label class="block text-white text-sm font-bold mb-2" for="cgpa">
                CGPA
            </label>
            <input
                class="shadow appearance-none border border-red-500 rounded w-full py-2 px-3 text-gray-700 mb-3 leading-tight focus:outline-none focus:shadow-outline"
                id="cgpa"
                type="text"
                placeholder="CGPA"
            />
        </div>

        <button
            class="bg-blue-500 hover:bg-blue-700 text-white font-bold py-2 px-4 rounded-full"
        >
            Save
        </button>
    </form>
</template>
