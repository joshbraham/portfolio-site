<svelte:head>
	<title>joshbraham.</title>
</svelte:head>

<section class="hero">
	<span class="greeting">Hello! My name is</span>
	<h1 class="name">Joshua <span class="lastname">Abraham.</span></h1>
	<p class="description">
		I am an aspiring frontend/backend/mobile/desktop/API etc. web developer & software engineer.
	</p>
	<div class="ctas">
		<a href="/contact" class="cta--primary"><i class="fa-regular fa-envelope" /> Contact Me</a>
		<a href="#" class="cta--cv"
			><span><i class="fa-regular fa-file-pdf" /> Download my CV</span><span>&rarr;</span></a
		>
	</div>
</section>

<hr />

<style>
	.hero {
		height: 35rem;
		line-height: 1;
		display: flex;
		flex-direction: column;
		gap: 1rem;
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
		font-size: 56px;
		font-weight: 900;
		letter-spacing: -0.04em;
		color: #ddd;
		word-spacing: 0.125em;
	}

	.lastname {
		color: var(--clr-accent);
	}

	.description {
		font-size: 24px;
		width: 44ch;
		line-height: 1.3;
	}

	.ctas {
		margin-top: 1.5rem;
		font-family: 'Chivo Mono', monospace;
		letter-spacing: 0.125em;
		text-transform: uppercase;
		display: flex;
		align-items: center;
		gap: 2rem;
	}

	.fa-envelope {
		position: relative;
		top: 1px;
	}

	.cta--cv {
		padding-block: 0.25em;
		/* margin-inline-start: 1em; */
		color: inherit;
		text-decoration: none;
		border-bottom: 1px solid currentColor;
		display: inline-flex;
		gap: 0.75em;
		transition: var(--default-transition);
	}

	.cta--cv:hover {
		color: var(--clr-primary);
		gap: 1.5em;
	}

	hr {
		width: 70vw;
		margin: 0 auto;
		border: none;
		border-top: 3px solid #555;
	}
</style>
