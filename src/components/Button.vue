<template>
    <button class="button"
        @click="$emit('onClick', label)"
        :class="{ double, triple, operation }">
        {{ label }}
    </button>
</template>

<script>
export default {
    props: {
        label: {},
        operation: { type: Boolean },
        double: { type: Boolean },
        triple: { type: Boolean },
    }
};
</script>

<style>
    :root { --bg-button: #f0f0f0; --border-button: solid 1px #888 }
    .button {
        cursor: pointer;
        font-size: 1.5rem;
        background-color: var(--bg-button);
        border: none;
        border-right: var(--border-button);
        border-bottom: var(--border-button);
        outline: none;
        transition: background .3s ease;
    }
    .button:hover { background-color: #fff }
    .button:active { background-color: #f0f0f0cc }
    .button.double { grid-column: span 2 }
    .button.triple { grid-column: span 3 }
    .button.operation { background: #fa8231 }
    .button.operation:active, .button.operation:hover { background: #fa8231cc }
</style>
