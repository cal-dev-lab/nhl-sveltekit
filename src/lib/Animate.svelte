<script>
    import { fly, fade } from "svelte/transition";
</script>

<div in:fly="{{ y: 200, duration: 2000 }}" out:fade>
    <slot></slot>
</div>