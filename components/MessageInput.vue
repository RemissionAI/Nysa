<script setup lang="ts">
const inputText = ref('');
const emit = defineEmits(['send-message']);

const sendMessage = () => {
    if (inputText.value.trim()) {
        emit('send-message', inputText.value);
        inputText.value = '';
    }
};
</script>

<template>
    <div class="message-input">
        <input v-model="inputText" @keyup.enter="sendMessage" type="text" placeholder="What can I help you with?" />
        <button @click="sendMessage" class="send-button">
            <Icon name="i-heroicons-paper-airplane" size="large" />
        </button>
    </div>
</template>

<style lang="scss" scoped>
.message-input {
    display: flex;
    background-color: var(--color-surface);
    border-radius: var(--border-radius-full);
    overflow: hidden;
    padding: 5px 10px;
    transition: border 0.1s ease;
    border: 1.4px solid var(--color-secondary);

    &:focus-within {
        border-color: var(--color-secondary-light);
    }

    input {
        flex-grow: 1;
        padding: 10px;
        font-size: 16px;
        margin-right: 10px;
        background: none;
        border: none;
        outline: none;
        color: var(--color-text-primary);
        font-family: var(--font-family-primary);

        &::placeholder {
            color: var(--color-text-secondary);
        }
    }

    .send-button {
        background-color: var(--color-background);
        color: var(--color-text-primary);
        border: none;
        border-radius: var(--border-radius-full);
        width: 40px;
        height: 40px;
        display: flex;
        align-items: center;
        justify-content: center;
        cursor: pointer;
    }
}
</style>