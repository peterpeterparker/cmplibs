<script lang="ts">
    import {createEventDispatcher} from 'svelte';

    export let color = '';

    const dispatch = createEventDispatcher();

    const yolo = () => dispatch('yolo')
</script>

<svelte:options tag="my-button"/>

<button on:click={yolo} style="background: {color}">Hello I'm a button</button>
