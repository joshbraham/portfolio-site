<svelte:head>
	<title>Welcome! &nbsp;|&nbsp; joshbraham.</title>
	<meta name="description" content="Joshua Abrahaam's developer profile." />
</svelte:head>

<section class="hero">
	<span class="greeting">Hello! My name is</span>
	<h1 class="name">Joshua <span class="lastname">Abraham.</span></h1>
	<p class="description">
		I am an aspiring frontend/backend/mobile/desktop/API etc. web developer & software engineer.
	</p>
	<div class="ctas">
		<a href="/contact" class="cta--contact">Contact Me <i class="fa-regular fa-envelope" /></a>
		<a href="#" class="cta--cv">Download my CV<span class="nbsp">&nbsp;&nbsp;</span>&rarr;</a>
	</div>
</section>

<hr />

<style>
	.hero {
		height: 35rem;
		display: flex;
		flex-direction: column;
		justify-content: center;
		background: rgba(0, 0, 0, 0.95) url('./hero-img.jpg');
		background-size: cover;
		background-blend-mode: color;
		padding-inline: var(--page-inline-padding);
		padding-block-start: var(--page-offset);
	}

	.hero > * {
		display: block;
		width: fit-content;
	}

	.greeting {
		font-family: 'Raleway', sans-serif;
		font-weight: bold;
		letter-spacing: 0.2em;
		color: #023afe;
		text-transform: uppercase;
	}

	.name {
		font-family: 'Raleway', sans-serif;
		font-size: 40px;
		font-weight: 900;
		letter-spacing: -0.04em;
		color: #ddd;
		word-spacing: 0.125em;
	}

	.lastname {
		color: #6800c3;
	}

	.description {
		font-size: 24px;
		width: 44ch;
		line-height: 1.3;
		/* color: white; */
	}

	.ctas > * {
		font-family: 'Raleway', sans-serif;
		font-size: 14px;
		font-weight: 800;
		letter-spacing: 4px;
		margin-top: 1.5rem;
		line-height: 1;
		display: inline-block;
		text-transform: uppercase;
		transition: all 150ms;
	}

	.cta--contact {
		color: white;
		padding: 1rem 1.5rem;
		background-color: #023afe;
		text-decoration: none;
		border-radius: 0.5rem;
	}

	.cta--contact:hover {
		background-color: hsl(227, 100%, 65%);
	}

	.cta--cv {
		padding: 1rem 1.5rem;
		color: #023afe;
		text-underline-offset: 4px;
	}

	.cta--cv:hover {
		color: inherit;
	}

	.nbsp {
		scale: 0.5 1;
	}

	.cta--cv:hover .nbsp {
		scale: 1;
	}

	hr {
		width: 70vw;
		margin: 0 auto;
		border: none;
		border-top: 3px solid #555;
	}
</style>
