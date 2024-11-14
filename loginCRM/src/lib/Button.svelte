<script>
    import { navigate } from "svelte-routing";

    export let btnText = "Iniciar";
    export let btnWidth = "50%";
    export let btnHeight = "60px";
    export let path = "/";
    export let btnBackgroundColor = "var(--color-beige)";

    function handleLoginClick() {
        navigate(path);
    }
</script>

<style>
    .personalizedBtn {
        font-size: 18px;
        border: none;
        cursor: pointer;
        color: var(--color-darkBrown);
    }
    .personalizedBtn:focus {
        outline: none;
    }
</style>

<button
    class="personalizedBtn"
    on:click={handleLoginClick}
    style="width: {btnWidth}; height: {btnHeight}; background-color: {btnBackgroundColor};"
>
    {btnText}
</button>
