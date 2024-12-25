<script>
    import NavBar from "./NavBar.svelte";
    import {animate, spring} from "motion"
    import { onMount } from "svelte";

    onMount(() => {
        animate(
            "h1",
            { y: [20, 0] },
        )
    });
</script>

<NavBar />
<section class="w-full h-3/4 bg-blue-500 rounded-[3rem]">
    <h1 class="font-bold text-4xl text-white">Milan Egberink</h1>
    <span class="font-['Excalifont']">Web dev</span>
</section>