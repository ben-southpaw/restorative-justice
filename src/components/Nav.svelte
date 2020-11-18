<script>
	//export let segment;
</script>
<section>
	<a class="icon" href="/"><span></span></a>
	<nav class="nav__container">
		<ul>
			<li><a href="work">Work</a></li>
			<li><a href="services">Services</a></li>
			<li><a href="about">About</a></li>
			<li><a href="stories">Stories</a></li>
			<div class="nav-contact">
				<li><a href="/">Contact</a> </li>
			</div>
		</ul>
	</nav>
</section>


<style lang="css">
	section {
		width: 100vw;
		height: 10vh;
		display: flex;
		justify-content: center;
		background: rgb(247, 247, 247);
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

	a:hover {
		color: black;
	}

	/* .current {
		text-decoration: underline;
	} */

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

	.icon:hover {
		opacity: 1;
	}

	/*.nav-menu {*/
	/*    display: none;*/
	/*    padding: 6px 4px;*/
	/*}*/

	.nav-contact {
		border-radius: 5px;
		padding: 6px 4px;
	}
</style>