<script>
	import './stylesheets/globals.css';
	import './stylesheets/reset.css';
</script>

<svelte:head>
	<meta name="description" content="Joshua Abraham's developer profile." />
</svelte:head>

<header>
	<div class="header-left">
		<a href="/"><svg class="logo"><use href="#logo" /></svg></a>
		<a href="https://github.com/joshbraham" target="_blank"
			><i class="fa-brands fa-github fa-lg" /></a
		>
		<a href="https://www.linkedin.com/in/joshuaabraham2804" target="_blank"
			><i class="fa-brands fa-linkedin fa-lg" /></a
		>
	</div>
	<nav>
		<ul class="nav-links">
			<li><a href="/about">About</a></li>
			<li><a href="/skills">Skills</a></li>
			<li><a href="/portfolio">Portfolio</a></li>
			<li><a href="/competencies">Competencies</a></li>
		</ul>
		<a class="cta--primary" id="nav-cta" href="/contact">Contact</a>
	</nav>
</header>

<main>
	<slot />
</main>

<footer>
	<!-- HIDDEN CONTENT -->
	<svg width="0" height="0" class="hidden">
		<symbol
			xmlns="http://www.w3.org/2000/svg"
			version="1.0"
			preserveAspectRatio="xMidYMid meet"
			viewBox="35 61 432.05 163.5"
			id="logo"
		>
			<g transform="translate(0.000000,250.000000) scale(0.100000,-0.100000)">
				<path
					d="M629 1867 c-95 -63 -86 -203 15 -251 95 -45 202 13 213 115 8 87 -58 159 -147 159 -32 0 -58 -7 -81 -23z"
				/>
				<path
					d="M1070 1375 c0 -478 -1 -495 -19 -505 -11 -5 -29 -10 -40 -10 -20 0 -21 -6 -21 -95 0 -93 1 -96 26 -105 38 -15 170 -12 208 4 19 8 44 28 56 44 l23 31 36 -29 c52 -42 112 -60 200 -60 109 0 164 21 232 89 64 64 93 129 111 247 14 89 1 209 -32 296 -26 70 -95 149 -155 178 -96 47 -229 42 -322 -11 l-53 -29 0 225 0 225 -125 0 -125 0 0 -495z m452 -105 c77 -22 124 -113 115 -226 -8 -102 -58 -169 -132 -175 -67 -5 -87 1 -125 39 -118 118 -56 358 95 371 6 1 27 -4 47 -9z"
				/>
				<path
					d="M2060 1270 l0 -600 125 0 125 0 0 248 c0 215 2 251 18 281 26 52 62 74 124 74 71 1 114 -23 139 -76 17 -38 19 -68 19 -284 l0 -243 125 0 125 0 0 243 c0 133 -5 273 -10 312 -19 128 -92 218 -207 251 -79 23 -206 20 -274 -6 -30 -11 -55 -20 -56 -20 -2 0 -3 95 -3 210 l0 210 -125 0 -125 0 0 -600z"
				/>
				<path
					d="M610 1493 c-19 -2 -50 -6 -67 -9 l-33 -5 0 -99 c0 -99 0 -100 24 -100 14 0 32 -7 41 -16 14 -15 16 -53 13 -353 -3 -325 -4 -337 -25 -371 -30 -48 -68 -68 -146 -76 l-67 -7 0 -94 c0 -80 3 -95 18 -101 9 -4 67 -7 127 -7 98 0 116 3 165 26 69 33 115 79 149 149 l26 55 0 430 c0 237 -3 442 -7 457 -10 34 -53 85 -87 102 -31 16 -82 23 -131 19z"
				/>
				<path
					d="M3089 1490 c-31 -4 -61 -10 -68 -14 -7 -5 -11 -42 -11 -102 l0 -94 28 0 c58 0 57 7 60 -315 l3 -295 119 0 120 0 0 260 c0 294 4 319 61 339 24 8 42 8 67 0 58 -19 62 -43 62 -339 l0 -260 119 0 120 0 3 274 c3 272 3 275 26 299 30 32 67 41 104 26 55 -22 58 -42 58 -334 l0 -265 126 0 126 0 -4 303 c-5 336 -9 360 -73 434 -88 103 -275 116 -392 27 l-33 -25 -33 25 c-55 42 -103 57 -185 57 -63 0 -85 -5 -133 -28 l-57 -29 -29 23 c-15 13 -44 26 -63 29 -19 3 -42 7 -50 8 -8 2 -40 0 -71 -4z"
				/>
				<path
					d="M4449 917 c-19 -12 -42 -38 -51 -57 -64 -126 76 -260 203 -195 95 50 92 213 -5 259 -49 23 -107 20 -147 -7z"
				/>
			</g>
		</symbol>
	</svg>
</footer>

<style>
	:global(body) {
		display: flex;
		flex-direction: column;
	}

	header {
		position: fixed;
		z-index: 10;
		top: 0;
		width: 100%;
		display: flex;
		justify-content: space-between;
		align-items: center;
		padding: 1rem var(--page-inline-padding);
	}

	.header-left {
		display: flex;
		align-items: center;
		gap: 1.5rem;
	}

	.header-left a {
		height: fit-content;
		line-height: 0;
	}

	.logo {
		height: 2rem;
		aspect-ratio: 2;
		position: relative;
		top: 2px;
		fill: var(--svg-color);
		transition: var(--default-transition);
	}

	.logo:hover {
		fill: var(--clr-accent);
	}

	.fa-brands {
		transition: var(--default-transition);
		color: var(--svg-color);
	}

	.fa-brands:hover {
		color: var(--clr-primary-light);
		scale: 1.1;
	}

	nav {
		/* height: fit-content; */
		/* border: 1px dashed red; */
		display: flex;
		gap: 1.5rem;
		font-family: 'Chivo Mono', monospace;
		font-size: 0.875rem;
		font-weight: 600;
	}

	.nav-links {
		/* border: 1px dashed green; */
		list-style: none;
		display: flex;
		align-items: center;
		gap: inherit;
	}

	.nav-links a {
		text-decoration: none;
		transition: var(--default-transition);
		position: relative;
		color: currentColor;
	}

	.nav-links a::after {
		content: '';
		position: absolute;
		left: 0;
		bottom: -2px;
		width: 100%;
		background: var(--clr-primary);
		height: 1px;
		transform-origin: top;
		transition: var(--default-transition);
	}

	.nav-links a:hover {
		color: var(--clr-primary);
	}

	.nav-links a:hover::after {
		scale: 1 3;
	}

	#nav-cta {
		padding: 0.5em 0.75em;
	}

	main {
		flex-grow: 1;
	}

	footer {
		background: white;
	}
</style>
