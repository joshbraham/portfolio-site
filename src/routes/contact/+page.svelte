<svelte:head>
	<title>Contact | joshbraham.</title>
</svelte:head>

<section>
	<form>
		<h1>Say Hello!</h1>
		<label for="email">Your Email Address</label>
		<input id="email" name="e" type="email" />

		<label for="occupation">I am a...</label>
		<select name="o" id="occupation" placeholder="Select an occupation">
			<option>select one...</option>
			<option>Recruiter</option>
			<option>Networker</option>
			<option>Tutor</option>
			<option>Other</option>
		</select>

		<label for="subject">Title</label>
		<input id="subject" name="s" type="text" />

		<label for="message">Message</label>
		<textarea id="message" name="m" rows="4" placeholder="Leave a message." />

		<button class="cta--primary" type="submit"
			>Send Away! <i class="fa-brands fa-telegram" /></button
		>
	</form>
</section>

<style>
	section {
		padding-inline: var(--page-inline-padding);
		padding-block-start: calc(var(--page-offset) + 1rem);
	}

	form {
		max-width: 30rem;
		margin: 0 auto;
		line-height: 1;
	}

	h1 {
		margin-block-end: 1.5rem;
	}

	label {
		font-family: 'Raleway', sans-serif;
		letter-spacing: 0.125em;
		font-weight: 600;
		text-transform: uppercase;
		font-size: 12px;
		color: var(--clr-primary-light);
		margin-block-end: 0.5rem;
	}

	label,
	input,
	textarea,
	select,
	button {
		display: block;
		width: 100%;
		border: none;
	}

	input,
	textarea,
	select {
		padding: 0.625rem;
		background: #333;
		margin-block-end: 1rem;
		border-bottom: 2px solid var(--clr-primary-light);
		border-radius: 0.25em;
		font-size: 16px;
	}

	button,
	select {
		cursor: pointer;
	}

	select:first-child {
		font-style: italic;
	}

	button {
		margin-top: 1.5rem;
		font-size: 16px;
		letter-spacing: 2px;
		text-transform: uppercase;
		font-family: 'Chivo Mono', monospace;
	}

	:is(input, textarea, select):focus {
		outline: 2px solid whitesmoke;
		border-color: #222;
	}

	textarea {
		resize: none;
		line-height: 1.2;
	}
</style>
