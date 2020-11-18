<script>
    import Nav from "../components/Nav.svelte";
    import { fade } from 'svelte/transition';

    let currentImageIndex = 0;

    const images = [
        '../images/imageOne.jpg',
        '../images/IMG_0979.jpg',
        '../images/IMG_0987.jpg',
        '../images/header_image.jpg'
    ]
    
    const next = () =>
        currentImageIndex = (currentImageIndex + 1) % images.length;

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
                    <li on:mouseover={next}>Your rights<span>Preview content</span></li>
                    <li on:mouseover={next}>Restorative Justice<span>Preview content</span></li>
                    <li on:mouseover={next}>Legal Aid<span>Preview content</span></li>
                    <li on:mouseover={next}>Next steps<span>Preview content</span></li>
                    <li on:mouseover={next}>Other links<span>Preview content</span></li>
                </ul>
            </div>
        </div>
        <div class="flex-container">
            {#each [images[currentImageIndex]] as photo (currentImageIndex)}
                <img src={photo} alt="gallery"/>
            {/each}
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
        margin-left: 20px;
    }

    img {
        display: inline-flex;
        width: 90%;
        height: 40vw;
        padding: 0 5%;
        object-fit: contain;
        /*opacity: 0;*/
        /*transition: opacity 0.2s;*/
    }

    /*.visible {*/
    /*    opacity: 1;*/
    /*}*/


</style>