<script>
    import { fade } from "svelte/transition";
    const name = "Tyler1 \u{1F1EF}\u{1F1F5}";
    const message = "Wait what ?";
    const img = "https://c.tenor.com/exTZBxFB6iMAAAAC/tyler1-loltyler1.gif";
</script>

<!-- absolute card -->
<div transition:fade class="z-10 text-neutral-100 p-4 absolute bottom-0 inset-x-0 w-full bg-blue-900/50">
    <h1 class="z-10 text-xl font-bold tracking-wide absolute top-0 -translate-y-7 inline-block px-4 rounded-t-lg bg-blue-900/50">{name}</h1>
    <img class="w-24 h-24 absolute top-0 left-0 -translate-y-full rounded-tr-lg -z-10" src={img} alt="Luna">
    <p class="first-letter:text-red-600 first-letter:font-bold z-10">{message} Lorem ipsum dolor sit amet, consectetur adipisicing elit. Exercitationem incidunt aliquam qui. Debitis corrupti ex veritatis illo, distinctio sunt repellendus, voluptatibus architecto sapiente quod iste laudantium nam. Est, soluta libero.</p>
</div>