<script>
    import WelcomeMessage from "../lib/WelcomeMessage.svelte";
    import StylishButton from "../lib/StylishButton.svelte";

    let name = "World"
</script>

<main>
<WelcomeMessage bind:name/>
<StylishButton bgColor="pink" txtColor="darkblue" message="I'm very stylish" functionToRun={()=>name = "Planet"}></StylishButton>
</main>

<style>
    main {
        display: flex;
        flex-direction: column;
        justify-content: center;
        align-items: center;
    }
</style>
