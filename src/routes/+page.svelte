<script lang="ts">
	import { fly } from 'svelte/transition'
</script>

<svelte:head>
	<title>Createhb21</title>
	<meta
		name="description"
		content="Createhb21 portfolio app | import createhb21 to 'your team'"
	/>
</svelte:head>

<section
	class='container'
	in:fly={{ x: -100, duration: 200, delay: 300 }}
	out:fly={{ x: -100, duration: 250 }}
>
	<!-- Header -->
	<header class="container">
		<hgroup>
			<h1>Createhb21 portfolio app</h1>
			<h2>
				import <b>createhb21</b>
				to <b>'your team'</b>
			</h2>
		</hgroup>
	</header>
	<!-- ./ Header -->

	<!-- Main -->
	<main class="container">
		<!-- Preview -->
		<section id="preview">
			<h2>Preview</h2>
			<p>Sed ultricies dolor non ante vulputate hendrerit. Vivamus sit amet suscipit sapien. Nulla iaculis eros a elit pharetra egestas.</p>
			<form>
				<div class="grid">
					<input type="text" name="firstname" placeholder="First name" aria-label="First name" required>
					<input type="email" name="email" placeholder="Email address" aria-label="Email address" required>
					<button type="submit">Subscribe</button>
				</div>
				<fieldset>
					<label for="terms">
						<input type="checkbox" role="switch" id="terms" name="terms">
						I agree to the <a href="../about">Privacy Policy</a>
					</label>
				</fieldset>
			</form>
		</section><!-- ./ Preview -->

		<!-- Typography-->
		<section id="typography">
			<h2>Typography</h2>
			<p>
				Aliquam lobortis vitae nibh nec rhoncus. Morbi
				mattis neque eget efficitur feugiat. Vivamus porta
				nunc a erat mattis, mattis feugiat turpis pretium.
				Quisque sed tristique felis.
			</p>

			<!-- Blockquote-->
			<blockquote>
				"Maecenas vehicula metus tellus, vitae congue turpis
				hendrerit non. Nam at dui sit amet ipsum cursus
				ornare."
				<footer>
					<cite>- Phasellus eget lacinia</cite>
				</footer>
			</blockquote>

			<!-- Lists-->
			<h3>Lists</h3>
			<ul>
				<li>
					Aliquam lobortis lacus eu libero ornare facilisis.
				</li>
				<li>Nam et magna at libero scelerisque egestas.</li>
				<li>
					Suspendisse id nisl ut leo finibus vehicula quis
					eu ex.
				</li>
				<li>
					Proin ultricies turpis et volutpat vehicula.
				</li>
			</ul>

			<!-- Headings-->
			<h3>Heading 3</h3>
			<p>
				Integer bibendum malesuada libero vel eleifend.
				Fusce iaculis turpis ipsum, at efficitur sem
				scelerisque vel. Aliquam auctor diam ut purus cursus
				fringilla. Class aptent taciti sociosqu ad litora
				torquent per conubia nostra, per inceptos himenaeos.
			</p>
		</section>
		<!-- ./ Typography-->

		<!-- Buttons-->
		<section id="buttons">
			<h2>Buttons</h2>
			<div class="grid">
				<button>Primary</button>
				<button class="secondary">Secondary</button>
				<button class="contrast">Contrast</button>
			</div>
			<div class="grid">
				<button class="outline">Primary outline</button>
				<button class="outline secondary"
					>Secondary outline</button
				>
				<button class="outline contrast"
					>Contrast outline</button
				>
			</div>
		</section>
		<!-- ./ Buttons -->

		<!-- Form elements-->
		<section id="form">
			<form>
				<h2>Form elements</h2>

				<!-- Search -->
				<label for="search">Search</label>
				<input
					type="search"
					id="search"
					name="search"
					placeholder="Search"
				/>

				<!-- Text -->
				<label for="text">Text</label>
				<input
					type="text"
					id="text"
					name="text"
					placeholder="Text"
				/>
				<small
					>Curabitur consequat lacus at lacus porta finibus.</small
				>

				<!-- Select -->
				<label for="select">Select</label>
				<select id="select" name="select" required>
					<option value="" selected>Select…</option>
					<option>…</option>
				</select>

				<!-- File browser -->
				<label for="file"
					>File browser
					<input type="file" id="file" name="file" />
				</label>

				<!-- Range slider control -->
				<label for="range"
					>Range slider
					<input
						type="range"
						min="0"
						max="100"
						value="50"
						id="range"
						name="range"
					/>
				</label>

				<!-- States -->
				<div class="grid">
					<label for="valid">
						Valid
						<input
							type="text"
							id="valid"
							name="valid"
							placeholder="Valid"
							aria-invalid="false"
						/>
					</label>
					<label for="invalid">
						Invalid
						<input
							type="text"
							id="invalid"
							name="invalid"
							placeholder="Invalid"
							aria-invalid="true"
						/>
					</label>
					<label for="disabled">
						Disabled
						<input
							type="text"
							id="disabled"
							name="disabled"
							placeholder="Disabled"
							disabled
						/>
					</label>
				</div>

				<div class="grid">
					<!-- Date-->
					<label for="date"
						>Date
						<input type="date" id="date" name="date" />
					</label>

					<!-- Time-->
					<label for="time"
						>Time
						<input type="time" id="time" name="time" />
					</label>

					<!-- Color-->
					<label for="color"
						>Color
						<input
							type="color"
							id="color"
							name="color"
							value="#0eaaaa"
						/>
					</label>
				</div>

				<div class="grid">
					<!-- Checkboxes -->
					<fieldset>
						<legend><strong>Checkboxes</strong></legend>
						<label for="checkbox-1">
							<input
								type="checkbox"
								id="checkbox-1"
								name="checkbox-1"
								checked
							/>
							Checkbox
						</label>
						<label for="checkbox-2">
							<input
								type="checkbox"
								id="checkbox-2"
								name="checkbox-2"
							/>
							Checkbox
						</label>
					</fieldset>

					<!-- Radio buttons -->
					<fieldset>
						<legend><strong>Radio buttons</strong></legend>
						<label for="radio-1">
							<input
								type="radio"
								id="radio-1"
								name="radio"
								value="radio-1"
								checked
							/>
							Radio button
						</label>
						<label for="radio-2">
							<input
								type="radio"
								id="radio-2"
								name="radio"
								value="radio-2"
							/>
							Radio button
						</label>
					</fieldset>

					<!-- Switch -->
					<fieldset>
						<legend><strong>Switches</strong></legend>
						<label for="switch-1">
							<input
								type="checkbox"
								id="switch-1"
								name="switch-1"
								role="switch"
								checked
							/>
							Switch
						</label>
						<label for="switch-2">
							<input
								type="checkbox"
								id="switch-2"
								name="switch-2"
								role="switch"
							/>
							Switch
						</label>
					</fieldset>
				</div>

				<!-- Buttons -->
				<input
					type="reset"
					value="Reset"
					on:click={(e) => e.preventDefault()}
				/>
				<input
					type="submit"
					value="Submit"
					on:click={(e) => e.preventDefault()}
				/>
			</form>
		</section>
		<!-- ./ Form elements-->

		<!-- Tables -->
		<section id="tables">
			<h2>Tables</h2>
			<figure>
				<table role="grid">
					<thead>
						<tr>
							<th scope="col">#</th>
							<th scope="col">Heading</th>
							<th scope="col">Heading</th>
							<th scope="col">Heading</th>
							<th scope="col">Heading</th>
							<th scope="col">Heading</th>
							<th scope="col">Heading</th>
							<th scope="col">Heading</th>
						</tr>
					</thead>
					<tbody>
						<tr>
							<th scope="row">1</th>
							<td>Cell</td>
							<td>Cell</td>
							<td>Cell</td>
							<td>Cell</td>
							<td>Cell</td>
							<td>Cell</td>
							<td>Cell</td>
						</tr>
						<tr>
							<th scope="row">2</th>
							<td>Cell</td>
							<td>Cell</td>
							<td>Cell</td>
							<td>Cell</td>
							<td>Cell</td>
							<td>Cell</td>
							<td>Cell</td>
						</tr>
						<tr>
							<th scope="row">3</th>
							<td>Cell</td>
							<td>Cell</td>
							<td>Cell</td>
							<td>Cell</td>
							<td>Cell</td>
							<td>Cell</td>
							<td>Cell</td>
						</tr>
					</tbody>
				</table>
			</figure>
		</section>
		<!-- ./ Tables -->

		<!-- Accordions -->
		<section id="accordions">
			<h2>Accordions</h2>
			<details>
				<summary>Accordion 1</summary>
				<p>
					Lorem ipsum dolor sit amet, consectetur adipiscing
					elit. Pellentesque urna diam, tincidunt nec porta
					sed, auctor id velit. Etiam venenatis nisl ut orci
					consequat, vitae tempus quam commodo. Nulla non
					mauris ipsum. Aliquam eu posuere orci. Nulla
					convallis lectus rutrum quam hendrerit, in
					facilisis elit sollicitudin. Mauris pulvinar
					pulvinar mi, dictum tristique elit auctor quis.
					Maecenas ac ipsum ultrices, porta turpis sit amet,
					congue turpis.
				</p>
			</details>
			<details open>
				<summary>Accordion 2</summary>
				<ul>
					<li>
						Vestibulum id elit quis massa interdum sodales.
					</li>
					<li>
						Nunc quis eros vel odio pretium tincidunt nec
						quis neque.
					</li>
					<li>
						Quisque sed eros non eros ornare elementum.
					</li>
					<li>
						Cras sed libero aliquet, porta dolor quis,
						dapibus ipsum.
					</li>
				</ul>
			</details>
		</section>
		<!-- ./ Accordions -->

		<!-- Article-->
		<article id="article">
			<h2>Article</h2>
			<p>
				Nullam dui arcu, malesuada et sodales eu, efficitur
				vitae dolor. Sed ultricies dolor non ante vulputate
				hendrerit. Vivamus sit amet suscipit sapien. Nulla
				iaculis eros a elit pharetra egestas. Nunc placerat
				facilisis cursus. Sed vestibulum metus eget dolor
				pharetra rutrum.
			</p>
			<footer>
				<small
					>Duis nec elit placerat, suscipit nibh quis,
					finibus neque.</small
				>
			</footer>
		</article>
		<!-- ./ Article-->

		<!-- Progress -->
		<section id="progress">
			<h2>Progress bar</h2>
			<progress id="progress-1" value="25" max="100" />
			<progress id="progress-2" />
		</section>
		<!-- ./ Progress -->

		<!-- Loading -->
		<section id="loading">
			<h2>Loading</h2>
			<article aria-busy="true" />
			<button aria-busy="true">Please wait…</button>
		</section>
		<!-- ./ Loading -->
	</main>
	<!-- ./ Main -->

	<!-- Footer -->
	<footer class="container">
		<small
			>Built with <a href="https://picocss.com">Pico</a> •
			<a
				href="https://github.com/picocss/examples/blob/master/basic-template/"
				>Source code</a
			></small
		>
	</footer>
	<!-- ./ Footer -->
</section>
