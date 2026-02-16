<script setup>
defineProps({
    promotion: String,
    storage: String,
    price: String,
    isPopular: Boolean
})
</script>

<template>

    <div :class="[
        'group w-75 rounded-xl text-white transition-all duration-300 border-10',
        isPopular
            ? 'border-[#a73fe3]'
            : 'border-[#62617284] hover:border-[#a73fe3]'
    ]">
        <div class="mb-10 text-center border-b-2 border-[#62617284] py-10">
            <h4 class="mb-10 font">{{ promotion }}</h4>
            <p class="mb-5 text-6xl font-serif">{{ storage }}</p>
            <p class="mb-5 ">{{ price }}</p>
            <button :class="[
                'mb-10 py-2 px-8 rounded-md transition-all duration-300 border',
                isPopular
                    ? 'bg-[#a73fe3] border-[#a73fe3]'
                    : 'border-[#a73fe3] group-hover:bg-[#a73fe3]'
            ]">
                Purchase
            </button>

        </div>
        <div class="text-center mb-10">
            <div class="flex justify-center items-center gap-4">
                <img src="./assets/check.png" alt="">
                <p>{{ storage }} storage</p>
            </div>
            <div class="flex justify-center items-center gap-4">
                <img src="./assets/check.png" alt="">
                <p>Option to add members</p>
            </div>
            <div class="flex justify-center items-center gap-4">
                <img src="./assets/check.png" alt="">
                <p>Extra member benefits</p>
            </div>
        </div>
    </div>

</template>

<style scoped></style>