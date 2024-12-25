<script>
    import {animate, stagger} from "motion";
    import {onMount} from "svelte";

    onMount(() => {
        animate("li", {opacity: [0, 1], y: [20, 0]}, {delay: stagger(0.05)});
    });
</script>

<nav class="flex items-center p-6 rounded-full m-4">
    <div class="h-full w-1/4 flex justify-center">
        <span class="font-medium text-2xl text-nowrap">Milan E.</span>
    </div>
    <div class="flex justify-center w-full">
        <ul class="flex text-xl gap-14 text-gray-500">
            <li>
                <a class="hover:text-gray-800 py-3 px-5 rounded-full hover:bg-gray-100 transition-all" href="/">Portfolio</a>
            </li>
            <li>
                <a class="hover:text-gray-800 py-3 px-5 rounded-full hover:bg-gray-100 transition-all"
                   href="/">Services</a>
            </li>
            <li>
                <a class="hover:text-gray-800 py-3 px-5 rounded-full hover:bg-gray-100 transition-all" href="/">Resources</a>
            </li>
            <li>
                <a class="hover:text-gray-800 py-3 px-5 rounded-full hover:bg-gray-100 transition-all"
                   href="/">Thoughts</a>
            </li>
        </ul>
    </div>
    <div class="h-full w-1/4 flex justify-center">
        <button class="text-nowrap bg-blue-400 text-white py-3 px-5 rounded-full hover:bg-blue-500">Got an idea?
        </button>
    </div>
</nav>