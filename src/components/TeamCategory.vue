<template>
<div class="max-w-sm bg-white border border-pink-300 rounded-lg shadow-md dark:bg-zinc-900 dark:border-pink-300">
    <a href="#">
        <img class="rounded-t-lg" :src="image" alt="" />
    </a>
    <div class="pt-8 pb-16 pl-8 pr-8">
        <a href="#">
            <h5 class="mb-2 text-2xl font-bold tracking-tight text-gray-900 dark:text-white">{{ name }}</h5>
        </a>
        <p class="mb-3 font-normal text-gray-700 dark:text-gray-400">{{ description }}</p>
    </div>
    <div class="absolute inset-x-0 bottom-0 h-12">
            <a href="#" class="inline-flex items-center px-3 py-2 text-sm font-medium text-center text-white bg-pink-300 rounded-lg hover:bg-pink-400 focus:ring-4 focus:outline-none focus:ring-pink-300 dark:bg-pink-300 dark:hover:bg-pink-300 dark:focus:ring-pink-800">
                Read more
                <svg aria-hidden="true" class="w-4 h-4 ml-2 -mr-1" fill="currentColor" viewBox="0 0 20 20" xmlns="http://www.w3.org/2000/svg"><path fill-rule="evenodd" d="M10.293 3.293a1 1 0 011.414 0l6 6a1 1 0 010 1.414l-6 6a1 1 0 01-1.414-1.414L14.586 11H3a1 1 0 110-2h11.586l-4.293-4.293a1 1 0 010-1.414z" clip-rule="evenodd"></path></svg>
            </a>
        </div>
</div>
</template>

<script>
export default {
    props: {
        image: String,
        description: String,
        name: String,
        socials: Array,
    },
};
</script>