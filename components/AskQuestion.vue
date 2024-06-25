<template>
    <div class="ask">
        <Icon name="brand-logo" size="3.5em"/>
        <div class="app-name">Nysa</div>
        <p class="app-description">Lupus AI assistant.</p>
        <MessageInput />
    </div>
</template>

<style lang="scss" >
.ask {
    max-width: 500px;
    width: 100%;
    display: flex;
    flex-direction: column;
    align-items: center;

    .app-name {
        font: var(--text-3xl-bold);
        font-family: var(--font-family-secondary);
    }

    .app-description {
        color: var(--color-text-secondary);
        margin-bottom: 2rem;
    }
}
</style>