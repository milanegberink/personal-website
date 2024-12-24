<script lang="ts">
    import {animate, stagger} from "motion"
    import {onMount} from "svelte";

    onMount(() => {
        animate(
            "li",
            { x: [-50, 0], opacity: [0,1] },
            { delay: stagger(0.1) }
        )

    });

    let test: number[] = [1, 2, 3, 4, 5, 6, 7, 8, 9];
</script>

{#each test as x}
    <li>{x}</li>
{/each}

