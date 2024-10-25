<template>

    <Head title="Products" />

    <FrontendLayout>
        <div class="mt-4 mx-4">
            <div class="flex justify-between">
                <h5>Show Product</h5>
                <Link :href="route('products.index')" class="bg-red-600 text-white py-2 px-5 rounded mb-4 inline-block">Back</Link>
            </div>
            <div class="grid grid-cols-12 gap-4">
                <div class="col-span-6">
                    <div class="mb-3">
                        <label>Product Name</label>
                        <p>{{product.name}}</p>
                    </div>
                </div>
                <div class="col-span-6">
                    <div class="mb-3">
                        <label>product Price</label>
                        <p>{{product.price}}</p>
                    </div>
                </div>
            </div>
        </div>
    </FrontendLayout>

</template>

<script setup>
    import FrontendLayout from '@/Layouts/FrontendLayout.vue';
    import { Head, Link, useForm } from '@inertiajs/vue3';
    defineProps({
        errors: Object ,
        product : Object
    });
</script>