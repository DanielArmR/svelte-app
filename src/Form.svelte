<script>
    const re = /^[\w-\.]+@([\w-]+\.)+[\w-]{2,4}$/g;
    $: validateEmail = true;
    const testInput = () => {
        let value = document.getElementById('email').value;
        return validateEmail = (re.test(value)) ? false : true;
    }
</script>

<form>
    <input type="text" id="email" placeholder="email" on:change={testInput}/>
    <button disabled={validateEmail}>Enviar</button>
</form>