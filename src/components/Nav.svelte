
<section>
	<div class="icon"></div>
	<nav class="nav__container">
		<ul>
			<li><a href="#">Work</a></li>
			<li><a href="#">Services</a></li>
			<li><a href="#">About</a></li>
			<li><a href="#">Stories</a></li>
<!--			<div class="nav-menu"><li>menu</li></div>-->

			<div class="nav-contact"><li><a href="#">Contact</a></li></div>
		</ul>
	</nav>
</section>


<style lang="scss">
	section {
		width: 100vw;
		height: 10vh;
		display: flex;
		justify-content: center;
		background: rgb(247,247,247);
		padding-top: 3vh;
		color: darkgray;
		position: absolute;
		top: 1.5vh;
	}

    nav {
        margin-left: auto;
        margin-right: 8vw;
        font-size: 14px;
    }

    ul {
        display: inline-flex;
        justify-content: space-between;
        }

    li {
        margin: auto 1.5vw;
        list-style-type: none;
        text-transform: uppercase;
        font-weight: 600;
    }

    a {
        text-decoration: none;
    }

	.icon {
		background-image: url(./../scale.svg);
		background-size: 35px;
		background-repeat: no-repeat;
		opacity: 0.4;
		height: 50px;
		width: 50px;
		display: inline-block;
		margin-left: 10vw;
        align-self: center;
	}

    .nav-menu {
        display: none;
        padding: 6px 4px;
    }

    .nav-contact {
        border-radius: 5px;
        padding: 6px 4px;
    }

</style>
