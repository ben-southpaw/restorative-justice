<script>
    // export let data
    import {fly} from 'svelte/transition';
    import {onMount} from 'svelte';

    export let data;

    let valueEntered = ``;

    onMount(() => {
        setTimeout(
            function () {
                valueEntered = 'there';
            }, 3000
        );

    });


</script>

<section>
    <header>
        {#if valueEntered}
            <h1 transition:fly="{{ y: 200, duration: 2000 }}">Hi {valueEntered} <br> welcome to Bowen Thornley Legal
            </h1>
        {/if}
    </header>
    <div class="header-footer">
        <div class="social-links">fb linkedIn etc</div>
        <h4>Auckland, New Zealand</h4>
    </div>

</section>


<style type="scss">

    section {
        width: 100vw;
        height: 90vh;
        //background: url(../header_image.jpg) no-repeat;
        //background-size: cover;
        background: rgb(247, 247, 247);
        text-align: center;
        padding: 1em;
        margin: 0 auto;
        margin-top: 10vh;

    }

    header {
        margin: 20vh 0;
    }

    h1 {
        text-transform: uppercase;
        font-size: 4em;
        font-weight: 100;
        margin: auto;
        margin-top: 10vh;
        width: 50%;
    }

    .header-footer {
        height: 30vh;
        margin-top: 20vh;
        display: flex;
        vertical-align: bottom;
    }

    .social-links {
        margin-left: 10vw;
        width: 50%;
        text-transform: uppercase;
        justify-content: space-between;
        color: darkgray;
        text-align: left;
    }

    h4 {
        width: 50%;
        color: darkgray;
        justify-content: space-between;
        text-transform: uppercase;
        text-align: right;

        margin-right: 10vw;
    }

</style>