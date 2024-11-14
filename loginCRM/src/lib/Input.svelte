<script>
    export let typeText = 'text';
    export let placeholder = '';

</script>

<input class="personalizedInput" type={typeText} placeholder={placeholder}>

<style>
    input{
        width: 100%;
        height: 50px;
        border: none;
        border-radius: 10px;
        padding: 0 20px;
        outline: none;
        font-size: 20px;
        background-color: #d9d9d9;
    }
</style>