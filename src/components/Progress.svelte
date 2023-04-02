<script>
// @ts-nocheck

    import { tweened } from 'svelte/motion';
	import { expoOut } from 'svelte/easing';
    import { onMount } from "svelte";

    const progress = tweened(0, {
		duration: 16000,
		easing: expoOut,
	});

    onMount(async () => {
        progress.set(100)
	});
</script>

<div class="progress active">
    <div class="progress-bar" role="progressbar" aria-valuenow="50" aria-valuemin="0" aria-valuemax="100" style="width: {$progress}%;">
    </div>
</div>