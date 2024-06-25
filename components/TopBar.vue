<script setup lang="ts">
defineEmits(['share']);
</script>

<template>
    <header class="top-bar">
        <div class="start">
            <NuxtLink to="/">
                <div class="logo">
                    <Icon name="i-brand-logo" size="3.2em" />
                </div>
            </NuxtLink>
        </div>
        <div class="end">
            <slot />
        </div>
    </header>
</template>

<style lang="scss" scoped>
.top-bar {
    display: flex;
    align-items: center;
    justify-content: start;
    padding: 10px 0;

    .end {
        margin-left: auto;
    }
}
</style>