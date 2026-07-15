<!-- 
Dark Mode:  ⏾ 
Light Mode: 𖤓
-->

<template>
<button @click="toggleDarkMode" class="bg-yellow-400 hover:bg-amber-400 text-black px-2 py-1 rounded-full">{{ light ? "𖤓" : "⏾" }}</button>
</template>

<script>
export default {
    data() {
        return {
            light: true
        };
    },
    methods: {
        toggleDarkMode() {
            this.light = !this.light;
            this.$emit('dark-switch');
        }
    }
};
</script>