<script>
    export let counter = 0;
    const increaseValue = () => {
        counter++;
    }
</script>

<h1>{counter}</h1>
<button on:click={increaseValue}>Increment</button>

<style>
    button{
        background-color: #ff3e00;
        border-radius: 10px;
        color: #fff;
        height: 8vh;
        width: 10vw;
        font-size: 1.4em;
        outline: none;
        border: none;
    }
</style>