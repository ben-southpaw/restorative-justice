<script>
    import Nav from "../components/Nav.svelte";

    let imgSrc = "../images/header_image.jpg";
</script>
<svelte:head>
    <title>Services</title>
</svelte:head>

<section>
    <div class="services-container">
        <Nav/>
        <div class="flex-container">
            <div class="title-container">
                <h1 class="title">Services</h1>
            </div>
            <div class="text-container">
                <ul>
                    <li>Your rights <span>Preview content</span></li>
                    <li>Our role <span>Preview content</span></li>
                    <li>Your costs <span>Preview content</span></li>
                    <li>Next steps <span>Preview content</span></li>
                    <li>Other links <span>Preview content</span></li>
                </ul>
            </div>
        </div>
        <div class="flex-container">
            <img src={imgSrc} alt="about image">
        </div>
    </div>

</section>

<style lang="scss">

    * {
        background: rgb(247, 247, 247);
    }

    section {
        padding-top: 10vh;
        height: 100vh;
    }

    .services-container {
        display: flex;
        margin: 0 auto;
        flex-direction: row;

    }

    .flex-container {
        width: 100vw;
        //height: 150vh;
    }

    .title-container {
        text-align: center;
        margin: 5vw;
        background: rgb(247, 247, 247);
        width: 40vw;
        height: 5vh;
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
        font-size: 21px;
        line-height: 36px;
        display: flex;
        flex-direction: row;
        text-align: center;
    }

    ul {
        width: 34vw;
    }

    span {
        display: none;

    }

    li {
        list-style-type: none;
        cursor: pointer;
    }

    li:hover span {
        display: inline-block;
    }

    img {
        display: inline-flex;
        width: 50vw;
        height: 40vw;
        object-fit: contain;
    }


</style>