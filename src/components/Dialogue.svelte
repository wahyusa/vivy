<script>
    import { fade } from "svelte/transition";
    const name = "Shiina \u{1F1FA}\u{1F1F8}";
    const message = "Hello World 😀";
    const img = "";
</script>

<!-- absolute card -->
<div transition:fade class="absolute inset-x-0 max-w-md top-1/2 z-10">
    <div class="bg-white rounded-md p-4">
    <slot name="title"></slot>
    <slot name="content"></slot>
    </div>
</div>