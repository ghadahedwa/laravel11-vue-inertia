<template>

        <Frontend>
            <Head title="AboutPage" />
        <h1>This is {{title}}</h1>
        </Frontend>
</template>

<script setup>
    import Frontend from '@/Layouts/FrontendLayout.vue';
    import { Head } from '@inertiajs/vue3';
    defineProps({
        title : String,
    });
</script>
