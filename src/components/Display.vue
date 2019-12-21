<template>
    <div class="display">{{ value }}</div>
</template>

<script>
export default {
    props: ['value']
};
</script>

<style>
    .display {
        display: flex;
        justify-content: flex-end;
        align-items: center;
        grid-column: span 4;
        background: #000;
        color: #fff;
        padding: 1rem;
        font-size: 2rem;
        overflow: hidden;
    }
</style>
