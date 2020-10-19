<script>
    export let data
    import { fly } from 'svelte/transition';

    let valueEntered = ``;


</script>

<section>
    <header>

            <input class="form__field" placeholder="Enter Your Name" bind:value={valueEntered}/>
        {#if valueEntered}
            <h1 transition:fly="{{ y: 200, duration: 3000 }}">Hi {valueEntered} <br> welcome to Bowen Thornley Legal</h1>
        {/if}
    </header>
</section>


<style type="scss">

    section {
        width: 100vw;
        height: 95vh;
        background: url(../header_image.jpg) no-repeat;
        background-size: cover;
        text-align: center;
        padding: 1em;
        margin: 0 auto;

    }

    h1 {
        text-transform: uppercase;
        font-size: 4em;
        font-weight: 100;
        margin: auto;
        width: 50%;
    }

    .form__field {
        font-family: inherit;
        border: 0;
        outline: 0;
        font-size: 1.3rem;
        color: dimgrey;
        text-transform: uppercase;
        padding: 7px 0;
        background: transparent;
        transition: border-color 0.2s;
        //visibility: hidden;
    }

    .form__field::first-letter {
        visibility: visible;
    }

    .form__field:hover {
        visibility: visible;
    }


</style>