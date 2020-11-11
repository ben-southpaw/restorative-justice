<script>
    import Nav from "../components/Nav.svelte";

    let imgSrc
    let src = '../images/header_image.jpg';
    let count = 0;
    let images = ['../images/header_image.jpg','../images/imageOne.jpg', '../images/IMG_0979.jpg', '../images/IMG_0987.jpg'];

    function handleMouseOver(e) {
         src = images[count++];
         if (count > 3) {
             count = 0;
             src = '../images/header_image.jpg';
         }
        console.log(count, 'count here');
    }

    console.log(count, 'log here')

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
                    <li on:mouseover={handleMouseOver}>Your rights <span>Preview content</span></li>
                    <li on:mouseover={handleMouseOver}>Our role <span>Preview content</span></li>
                    <li on:mouseover={handleMouseOver}>Your costs <span>Preview content</span></li>
                    <li on:mouseover={handleMouseOver}>Next steps <span>Preview content</span></li>
                    <li on:mouseover={handleMouseOver}>Other links <span>Preview content</span></li>
                </ul>
            </div>
        </div>
        <div class="flex-container">
            <!--{#if hovered}-->
            <img {src} alt="about image">
            <!--{/if}-->
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
        width: 90%;
        height: 40vw;
        padding: 0 5%;
        object-fit: contain;
    }


</style>