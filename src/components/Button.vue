<script setup>
    const props = defineProps({
        operador: String,
        fn: Function
    });

    console.log(props);
</script>

<template>
    <button
        type="button"
        class="h-10 w-10 flex items-center justify-center font-bold bg-violet-500 rounded-full hover:outline-none hover:ring-2 hover:ring-offset-2 hover:ring-violet-500 text-white text-2xl"
        @click="$emit('fn')"
    >{{ operador }}</button>
</template>