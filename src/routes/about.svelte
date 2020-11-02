<script>
    import Nav from "../components/Nav.svelte";
</script>
<svelte:head>
    <title>About</title>
</svelte:head>

<section>
    <div class="about-container">
        <Nav/>
        <div class="title-container">
            <h1 class="title">About Us</h1>
        </div>
        <div class="text-container">
            <p>Lorem ipsum dolor sit amet, consectetur adipisicing elit. Blanditiis
                dignissimos eaque eius numquam quasi quo totam!
                Ad commodi consequuntur ex facere, illo, iure maiores, nemo odit
                perferendis quam rem voluptate!Lorem ipsum dolor sit amet, consectetur
                adipisicing elit. A ab animi at atque beatae commodi dignissimos dolores
                dolorum eos expedita incidunt ipsam ipsum laudantium molestiae nihil,
                quia quos, repellendus, voluptates.</p>
        </div>
        <img src="./../header_image.jpg" alt="about image">
        <div class="text-container">
            <p>Lorem ipsum dolor sit amet, consectetur adipisicing elit. Blanditiis
                dignissimos eaque eius numquam quasi quo totam!
                Ad commodi consequuntur ex facere, illo, iure maiores, nemo odit
                perferendis quam rem voluptate!Lorem ipsum dolor sit amet, consectetur
                adipisicing elit. A ab animi at atque beatae commodi dignissimos dolores
                dolorum eos expedita incidunt ipsam ipsum laudantium molestiae nihil,
                quia quos, repellendus, voluptates.</p>
        </div>
    </div>

</section>

<style lang="scss">

    * {
        background: rgb(247, 247, 247);
    }

    section {
        padding-top: 10vh;
    }

    .about-container {
        display: flex;
        flex-direction: column;
        //height: 100vh;
        max-width: 1400px;
        margin: 0 auto;

    }

    .title-container {
        padding-top: 15vh;
        width: 60vw;
        margin: 0 auto;
        background: rgb(247,247,247);
    }

    h1 {
        font-size: 48px;
        color: darkgray;
    }

    .text-container {
        width: 60vw;
        height: 50vh;
        margin: 0 auto;
        background: rgb(247,247,247);
        border-radius: 7px;
        font-size: 21px;
        line-height: 36px;
    }

    img {
        display: block;
        width: 100vw;
        height: 40vw;
        object-fit: contain;
        margin-bottom: 15vh;
    }


</style>