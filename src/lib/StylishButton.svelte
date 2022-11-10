<script>
    export let bgColor = "grey"
    export let txtColor = "black"
    export let message = ""
    export let functionToRun = () => console.log("I'm a stylish button")
</script>

<button style="--bgColor:{bgColor}; --txtColor:{txtColor}" on:click={functionToRun}>{message}</button>

<style>
    button {
        border: none;
        background: var(--bgColor);
        color: var(--txtColor);
        padding: 20px;
        border-radius: 8px;
        transition: 0.3s ease-in-out;
    }

    button:hover {
        filter: brightness(120%);
    }
</style>
