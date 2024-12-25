<script>
    import {animate, stagger} from "motion";
    import {onMount} from "svelte";

    onMount(() => {
        animate("li", {opacity: [0, 1], y: [20, 0]}, {delay: stagger(0.05)});
    });
</script>

<nav class="border flex items-center p-10">
    <span class="font-medium text-2xl">Milan</span>
    <div class="flex justify-center w-full">
        <ul class="flex text-xl gap-14 text-gray-500">
            <li>
                <a class="hover:text-gray-800 py-3 px-5 rounded-full hover:bg-gray-100 transition-all" href="/">Portfolio</a>
            </li>
            <li>
                <a class="hover:text-gray-800 py-3 px-5 rounded-full hover:bg-gray-100 transition-all" href="/">Services</a>
            </li>
            <li>
                <a class="hover:text-gray-800 py-3 px-5 rounded-full hover:bg-gray-100 transition-all" href="/">Resources</a>
            </li>
            <li>
                <a class="hover:text-gray-800 py-3 px-5 rounded-full hover:bg-gray-100 transition-all" href="/">Thoughts</a>
            </li>
        </ul>
    </div>
    <button class="text-nowrap bg-blue-400 text-white py-3 px-5 rounded-full hover:bg-blue-500">Got an idea?</button>
</nav>