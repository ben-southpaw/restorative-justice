<script>
    import Nav from "../components/Nav.svelte";
</script>
<svelte:head>
    <title>Work</title>
</svelte:head>

<section>
    <div class="stories-container">
        <Nav/>
        <div class="flex-container">
            <div class="title-container">
                <h1 class="title">Work example</h1>
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
            <img src="../images/header_image.jpg" alt="work">
        </div>

        <div class="flex-container">
            <img src="../images/header_image.jpg" alt="work">
            <div class="title-container">
                <h1 class="title">Work Example 2</h1>
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

    .stories-container {
        display: flex;
        margin: 0 auto;

    }

    .flex-container {
        width: 100vw;
        //height: 150vh;
    }

    .title-container {
        padding-top: 5vh;
        margin: 0 5vw;
        background: rgb(247, 247, 247);
    }

    h1 {
        font-size: 48px;
        color: darkgray;
    }

    .text-container {
        width: 40vw;
        height: 40vh;
        margin:5vw;
        background: rgb(247, 247, 247);
        border-radius: 7px;
        font-size: 21px;
        line-height: 36px;
        display: flex;
        flex-direction: row;
    }

    img {
        display: inline-flex;
        width: 90%;
        height: 40vw;
        padding: 0 5%;
        object-fit: contain;
    }


</style>