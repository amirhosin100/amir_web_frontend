<script setup>
const props = defineProps({
    title:{
        default:"Terminal"
    }
})

</script>

<template>
    <div class="overflow-hidden rounded-2xl border border-neutral-200 bg-[#0d0f14] shadow-2xl dark:border-white/10">
        <div class="relative flex items-center gap-2 border-b border-white/10 px-4 py-3">
        <span class="h-3 w-3 rounded-full bg-[#ff5f57]"></span>
        <span class="h-3 w-3 rounded-full bg-[#febc2e]"></span>
        <span class="h-3 w-3 rounded-full bg-[#28c840]"></span>
        <span class="pointer-events-none absolute inset-x-0 text-center font-mono text-xs text-white/40">{{ title }}</span>
        </div>
        <slot></slot>
    </div>
</template>