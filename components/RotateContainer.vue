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
    overflow: hidden;
    border-radius: var(--border-radius-full);

    &::before {
        content: "";
        display: block;
        background: linear-gradient(90deg,
                rgba(255, 255, 255, 0) 0%,
                rgb(102, 102, 102) 50%,
                rgba(255, 255, 255, 0) 100%);
        height: 100%;
        width: 100px;
        transform: translate(0);
        position: absolute;
        animation: rotate 5s linear forwards infinite;
        z-index: 0;
        top: 50%;
        transform-origin: top center;
    }

    .inner {
        position: relative;
        z-index: 10;
        width: 100%;
        margin: .5px;
    }

}
</style>