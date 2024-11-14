<script>
    let isOn = false;

    function toggle() {
        isOn = !isOn;
    }
</script>

<style>
    .toggleBtn {
        width: 70px;
        background-color: #f5f3f1;
        border-radius: 25px;
        padding: 3px;
        border: 2px solid #917161;
        outline: none;
    }
    .toggleBtn__ball {
        height: 25px;
        aspect-ratio: 1/1;
        background-color: #917161;
        border-radius: 100%;
        transition: all 0.3s ease;
    }
    .toggleBtn.isOn .toggleBtn__ball {
        transform: translateX(35px);
        background-color: #f5f3f1;
        
    }
    .toggleBtn.isOn  {
        background-color: #917161;
        
    }
</style>

<button class="toggleBtn" on:click={toggle} class:isOn>
    <div class="toggleBtn__ball"></div>
</button>
