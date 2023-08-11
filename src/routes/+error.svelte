<svelte:head>
	<title>???</title>
</svelte:head>

<section>
	<svg class="logo"><use href="#logo" /></svg>
	<p>Coming soon... 🤩</p>
</section>

<style>
	section {
		--backdrop-color: rgb(54, 54, 54);
		padding-block-start: calc(var(--page-offset) + 10rem);
		padding-inline: var(--page-inline-padding);
		font: 4em 'Chivo Mono';
		height: 100%;
		position: relative;
	}

	svg {
		position: absolute;
		z-index: -1;
		top: 50%;
		left: 50%;
		translate: -50% -50%;
		aspect-ratio: 2;
		width: 50%;
		fill: transparent;
		stroke: var(--backdrop-color);
		stroke-width: 20;
		stroke-dasharray: 6500;
		stroke-dashoffset: 6500;
		animation: draw 4s infinite;
	}

	@keyframes draw {
		30% {
			fill: transparent;
		}
		50% {
			stroke-dashoffset: 13000;
			fill: var(--backdrop-color);
		}
		70% {
			fill: transparent;
		}
		100% {
			stroke-dashoffset: 19500;
		}
	}
</style>
