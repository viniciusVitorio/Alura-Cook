<script lang="ts">
    export let tag: 'h1' | 'h2' | 'h3' | 'h4' | 'h5' | 'h6'
</script>

<svelte:element class="titulo" this={tag}>
    <slot></slot>
</svelte:element>

<style>
     .titulo {
        color: var(--verde);
        text-transform: uppercase;
        font-size: 1.5rem;
        font-weight: 700;
        line-height: 2rem;
        margin-bottom: 1rem;
        margin-top: 2rem;
    }
</style>