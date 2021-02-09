<script>
    export let counter = 0;
    const increaseValue = () => {
        counter++;
    }
    //Con el signpo de dolar y dos puntos le decimos a svelte que esa sentencia es reactiva
    $: isEvenOrOdd = counter % 2 === 0 ? 'Is Even' : 'Is Odd';
</script>

<h1>{counter}</h1>
<button on:click={increaseValue}>Increment</button>
<h2>{isEvenOrOdd}</h2>

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