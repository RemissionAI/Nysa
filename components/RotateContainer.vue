<template>
    <div class="rotate-container">
        <div class="inner">
            <slot/>
        </div>
    </div>
    
</template>

<style lang="scss" scoped>

.rotate-container {
    position: relative;
    display: flex;
    align-items: center;
    justify-content: center;
    overflow: hidden;
    border-radius: var(--border-radius-full);
    width: 100%;

    &::before {
        content: "";
        display: block;
        background: linear-gradient(90deg,
                rgba(255, 255, 255, 0) 0%,
                rgb(102, 102, 102) 50%,
                rgba(255, 255, 255, 0) 100%);
        width: 100%;
        height: 200px;
        transform: translate(0);
        position: absolute;
        animation: rotate 6s linear forwards infinite;
        z-index: 0;
        top: 50%;
        transform-origin: bottom center;
    }

    .inner {
        position: relative;
        z-index: 10;
        width: 100%;
        margin-top: .8px;
        margin-bottom: .32px;
    }

}
</style>