<script>

export let btnText = "Iniciar";
export let btnWidth = "50%";
export let btnHeight = "60px";
export let onClick = () => {};

</script>

<button on:click={onClick} style="width: {btnWidth}; height: {btnHeight}; ">
    {btnText}
</button>

<style>

</style>