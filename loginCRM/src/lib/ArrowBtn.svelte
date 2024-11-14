<script>
    import { navigate } from "svelte-routing";

    export let path = "/";
    export let svgColor = "var(--color-cream)";

    function handleArrowClick() {
        navigate(path);
    }
</script>

<style>
    button {
        padding: 0;
        background-color: transparent;
    }
    .arrowBtn {
        height: 75px;
    }
    svg {
        height: 100%;
    }
</style>

<button class="arrowBtn" on:click={handleArrowClick}>
    <svg viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg"
        ><g id="SVGRepo_bgCarrier" stroke-width="0"></g><g
            id="SVGRepo_tracerCarrier"
            stroke-linecap="round"
            stroke-linejoin="round"
        ></g><g id="SVGRepo_iconCarrier">
            <path
                d="M6 12H18M6 12L11 7M6 12L11 17"
                stroke={svgColor}
                stroke-width="2"
                stroke-linecap="round"
                stroke-linejoin="round"
            ></path>
        </g></svg
    >
</button>
