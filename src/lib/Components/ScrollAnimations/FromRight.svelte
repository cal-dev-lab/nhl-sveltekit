<script>
    import Saos from "saos";
</script>

<Saos animation={'from-right 2s cubic-bezier(0.35, 0.5, 0.65, 0.95) both'}>
<slot></slot>
</Saos>

<style>
    @keyframes -global-from-right {
        0% {
            transform: rotateX(50deg) translateX(200vw) skewX(-50deg);
            opacity: 1;
        }
        100% {
            transform: rotateX(0deg) translateX(0) skewX(0deg);
            opacity: 1;
        }
    }
</style>