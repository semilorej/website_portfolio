<script>
	import 'bootstrap/dist/css/bootstrap.min.css'; // Import Bootstrap CSS
	import 'jquery/dist/jquery.min.js';

	let testimonials = [
		{
			id: 1,
			text: "Semilore is a talented developer who delivers high-quality work on time. I'm impressed by his dedication to excellence.",
			author: 'Amupitan Samuel',
			position: 'Front-end Developer'
		},
		{
			id: 2,
			text: "Semilore is a true visionary with an unparalleled dedication to excellence, always pushing the boundaries with creativity and determination. It's a privilege to witness your outstanding work ethic and unwavering commitment to sucess",
			author: 'Adeolu John',
			position: 'Chemical Engineer'
		},
		{
			id: 3,
			text: "Semilore's problem-solving skills and attention to detail are exceptional. It's a pleasure to work with him.",
			author: 'Jane Smith',
			position: 'Senior Designer'
		},
		{
			id: 4,
			text: 'Semilore is a very talented, diligent and a go getter, always ready to solve problems.',
			author: 'Oyewale Mojola',
			position: 'CEO Ornate.ng'
		}

		// Add more testimonials here
	];

	// Particle.js configuration
	let particlesConfig = {
		particles: {
			number: {
				value: 100,
				density: {
					enable: true,
					value_area: 800
				}
			},
			color: {
				value: '#000000' // Adjust the particle color
			},
			shape: {
				type: 'circle'
			},
			opacity: {
				value: 0.7,
				random: false,
				anim: {
					enable: false,
					speed: 1,
					opacity_min: 0.1,
					sync: false
				}
			},
			size: {
				value: 3,
				random: true,
				anim: {
					enable: false,
					speed: 40,
					size_min: 0.1,
					sync: false
				}
			}
		},
		interactivity: {
			detect_on: 'canvas',
			events: {
				onhover: {
					enable: true,
					mode: 'repulse'
				}
			}
		}
	};

	import { onMount } from 'svelte';

	onMount(() => {
		particlesJS('particles-js', particlesConfig);
	});
</script>

<main>
	<div id="particles-js" class="animated-background" />

	<!-- Navbar -->
	<nav class="navbar navbar-expand-lg navbar-light bg-transparent text-dark">
		<div class="container">
			<a class="navbar-brand brand-name" href="/">Semilore</a>
			<button
				class="navbar-toggler"
				type="button"
				data-bs-toggle="collapse"
				data-bs-target="#navbarNav"
			>
				<span class="navbar-toggler-icon" />
			</button>
			<div class="collapse navbar-collapse" id="navbarNav">
				<ul class="navbar-nav ms-auto">
					<li class="nav-item">
						<a class="nav-link" href="#about">About</a>
					</li>
					<li class="nav-item">
						<a class="nav-link" href="#portfolio">Portfolio</a>
					</li>
					<li class="nav-item">
						<a class="nav-link" href="#testimonials">Testimonials</a>
					</li>
					<li class="nav-item">
						<a href="#contact" class="btn btn-white btn-md rounded-pill text-black d-inline-block">
							Get in touch <i class="fas fa-arrow-right" />
						</a>
					</li>
				</ul>
			</div>
		</div>
	</nav>

	<!-- Introduction Section -->
	<section class="intro text-start text-dark py-4">
		<div class="container">
			<div class="row">
				<div class="col-md-7 d-flex align-items-center">
					<div>
						<!-- Update the text color to purple -->
						<h1 class="display-3 fw-bolder text-white">
							Hi! I'm <span class="text-purple">Semilore</span>
						</h1>
						<h1 class="display-5 fw-bold text-white" style="margin-top: -20px;">
							Front-end<span class="text-purple">Developer</span>
						</h1>
						<p class="text-white" style="margin-top: 20px;">
							My <span class="text-purple">favourite tech</span> includes JavaScript (REACT.JS), Svelte
							and Sveltekit, BootstrapCSS, Node.js.
						</p>
						<!-- Update the button styles with the arrow icon -->
						<a
							href="#portfolio"
							class="btn btn-white btn-md rounded-pill text-black d-inline-block"
							style="margin-top: 20px;">View Portfolio</a
						>
						<a
							href="#contact"
							class="btn btn-white btn-md rounded-pill text-black d-inline-block"
							style="margin-top: 20px;"
						>
							Get in touch <i class="fas fa-arrow-right" />
						</a>
					</div>
				</div>
				<div class="col-md-5 ms-auto d-flex align-items-center">
					<div class="mx-auto">
						<!-- Center the image within its container -->
						<!-- Add your picture here -->
						<img
							src="/DSC_0750-removebg-preview.png"
							alt="Your Name"
							class="img-fluid rounded-circle mb-3"
						/>
					</div>
				</div>
			</div>
		</div>
	</section>

	<hr class="my-5 mx-auto" style="width: 70%; border-top: 4px solid white;" />

	<!-- About Me Section -->
	<section id="about" class="section py-5">
		<div class="container">
			<!-- Section 1 -->
			<div class="row mb-5">
				<div class="col-md-4 text-white d-flex align-items-center justify-content-center">
					<h1 class="display-1 fw-bolder text-purple">01</h1>
				</div>
				<div class="col-md-8 text-white">
					<h2 class="mb-4">A bit about me</h2>
					<p style="text-align: justify;">
						Hi! I'm Oyewale Semilore, a passionate and creative web developer with a focus on
						crafting interactive and user-friendly websites. With a solid foundation in HTML, CSS,
						and JavaScript, I bring a unique blend of technical skills and a keen eye for design to
						every project.
					</p>
				</div>
			</div>

			<!-- Section 2 -->
			<div class="row mb-5">
				<div class="col-md-4 text-white d-flex align-items-center justify-content-center">
					<h1 class="display-1 fw-bolder text-purple">02</h1>
				</div>
				<div class="col-md-8 text-white">
					<h2 class="mb-4">Tech Stack</h2>
					<p style="text-align: justify;">
						My journey in web development began with a strong desire to create digital experiences
						that leave a lasting impact. Over the years, I have honed my skills in front-end
						technologies, specializing in frameworks like React.js and Svelte. I am also well-versed
						in utilizing BootstrapCSS to ensure responsive and visually appealing designs.
					</p>
				</div>
			</div>

			<!-- Section 3 -->
			<div class="row">
				<div class="col-md-4 text-white d-flex align-items-center justify-content-center">
					<h1 class="display-1 fw-bolder text-purple">03</h1>
				</div>
				<div class="col-md-8 text-white">
					<h2 class="mb-4">Commitment to Excellence</h2>
					<p style="text-align: justify;">
						What sets me apart is my commitment to continuous learning and staying updated with the
						latest industry trends. I believe in the power of collaboration and enjoy turning ideas
						into functional and aesthetically pleasing websites.
					</p>
				</div>
			</div>
		</div>
	</section>
	<!-- Portfolio Section (Separate Cards) -->
	<section id="portfolio" class="section bg-light py-5">
		<div class="container">
			<h2 class="mb-4 text-center">Portfolio</h2>
			<div class="row">
				<!-- Card 1 -->
				<div class="col-md-4 mb-4">
					<div class="card h-100 border-0 shadow">
						<img
							src="/Eye_product.png"
							class="card-img-top"
							alt="Project 1"
							style="height: 200px;"
						/>
						<div class="card-body">
							<h5 class="card-title">Eye Product Store</h5>
							<p class="card-text">
								The Eye Product Store project is a visually engaging and user-friendly e-commerce
								platform designed and developed by me. It features a sleek and modern design to
								showcase a variety of eye-related products, including glasses, contact lenses, and
								accessories.
							</p>
							<a href="your_link_for_project_1" class="btn btn-purple rounded-pill">Details</a>
						</div>
					</div>
				</div>

				<!-- Card 2 -->
				<div class="col-md-4 mb-4">
					<div class="card h-100 border-0 shadow">
						<img src="/Todo.png" class="card-img-top" alt="Project 2" style="height: 200px;" />
						<div class="card-body">
							<h5 class="card-title">To-do List App</h5>
							<p class="card-text">
								The TodoList App project is a practical and efficient task management tool that I
								developed as part of my web development portfolio. It offers a clean and intuitive
								user interface, allowing users to easily create, organize, and prioritize their
								tasks. The app includes features such as task categorization, due dates, and the
								ability to mark tasks as complete.
							</p>
							<a href="https://todolistbysemilore.vercel.app/" class="btn btn-purple rounded-pill"
								>Details</a
							>
						</div>
					</div>
				</div>

				<!-- Card 3 -->
				<div class="col-md-4 mb-4">
					<div class="card h-100 border-0 shadow">
						<img src="/calculator.png" class="card-img-top" alt="Project 3" />
						<div class="card-body">
							<h5 class="card-title">Calculator app</h5>
							<p class="card-text">
								The Calculator App project is a functional and user-friendly application that I
								developed for my web development portfolio. It provides a sleek and responsive
								interface for performing basic arithmetic operations such as addition, subtraction,
								multiplication, and division. The calculator includes a clear display, easy-to-use
								buttons, and a responsive design for seamless use on various devices.
							</p>
							<a href='https://semilorecalculator.vercel.app/' class="btn btn-purple rounded-pill">Details</a>
						</div>
					</div>
				</div>
			</div>
		</div>
	</section>
	<!-- Testimonials Section -->
	<section id="testimonials" class="section bg-light py-5">
		<div class="container">
			<h2 class="mb-4 text-center">Testimonials</h2>
			<div class="row">
				{#each testimonials as testimonial (testimonial.id)}
					<div class="col-md-6">
						<p style="text-justify: auto;">{testimonial.text}</p>
						<small class="text-muted">
							- {testimonial.author}, {testimonial.position}
						</small>
					</div>
				{/each}
			</div>
		</div>
	</section>

	<!-- Contact Me Section -->
	<section id="contact" class="section py-5">
		<div class="container text-white">
			<div class="row">
				<div class="col-md-6">
					<h3 class="mb-4">Get in touch</h3>
					<fieldset>
						<legend class="visually-hidden">Contact Form</legend>
						<p class="mb-4">Feel free to send me a message using the contact form below:</p>
						<form action="https://formspree.io/f/xjvqdgnl" method="POST">
							<div class="mb-3">
								<label for="name" class="form-label">Name</label>
								<input
									type="text"
									id="name"
									name="name"
									class="form-control"
									placeholder="Your Name"
									required
								/>
							</div>
							<div class="mb-3">
								<label for="email" class="form-label">Email</label>
								<input
									type="email"
									id="email"
									name="email"
									class="form-control"
									placeholder="Your Email"
									required
								/>
							</div>
							<div class="mb-4">
								<label for="message" class="form-label">Message</label>
								<textarea
									id="message"
									name="message"
									class="form-control"
									placeholder="Your Message"
									rows="4"
									required
								/>
							</div>
							<button type="submit" class="btn btn-purple rounded-pill">Submit</button>
						</form>
					</fieldset>
				</div>
				<div class="col-md-6 d-flex align-items-center justify-content-center">
					<!-- <h3 class="mb-4">You can reach me on:</h3> -->
					<ul class="list-unstyled">
						<li>Email: oyewaleoluwasemilore.com</li>
						<li>Phone: +(234) 8174070138</li>
						<li>
							LinkedIn: <a href="https://www.linkedin.com/in/semiloreoye"
								>linkedin.com/in/semiloreoye</a
							>
						</li>
						<li>
							GitHub: <a href="https://www.https://github.com/semilorej">github.com/semilorej</a>
						</li>
					</ul>
				</div>
			</div>
		</div>
	</section>

	<!-- Footer Section -->
	<footer class="footer bg-dark text-white py-4">
		<div class="container">
			<div class="row">
				<div class="col-md-6 text-center text-md-start">
					<p>&copy; 2023 Semilore</p>
				</div>
				<div class="col-md-6 text-center text-md-end">
					<ul class="list-inline social-icons">
						<!-- <li class="list-inline-item">
							<a href="#" class="social-icon-link">
								<i class="fab fa-facebook" aria-label="Facebook" style="color: white;" />
							</a>
						</li> -->
						<li class="list-inline-item">
							<a href="https://twitter.com/theSemilore__" class="social-icon-link">
								<i class="fab fa-twitter" aria-label="Twitter" style="color: white;" />
							</a>
						</li>
						<li class="list-inline-item">
							<a href="https://www.linkedin.com/in/semiloreoye" class="social-icon-link">
								<i class="fab fa-linkedin" aria-label="LinkedIn" style="color: white;" />
							</a>
						</li>
						<li class="list-inline-item">
							<a href="https://www.https://github.com/semilorej" class="social-icon-link">
								<i class="fab fa-github" aria-label="GitHub" style="color: white;" />
							</a>
						</li>
						<!-- Add more social icons as needed, and apply the "style" attribute with "color: white;" to each one -->
					</ul>
				</div>
			</div>
		</div>
	</footer>
</main>

<slot />

<style>
	/* Add a custom class for purple text color */
	.text-purple {
		color: #663399;
	}

	/* The rest of your existing styles */
	.brand-name {
		font-size: 2rem;
		color: white; /* Change the color to white */
	}

	.animated-background {
		position: fixed;
		top: 0;
		left: 0;
		width: 100%;
		height: 100%;
		z-index: -1;
		background: #000033; /* Deep blue color */
	}

	/* Update the link color to white */
	.navbar .navbar-nav .nav-link {
		color: white;
	}

	/* Update the link color when hovered to a different color (e.g., gray) */
	.navbar .navbar-nav .nav-link:hover {
		color: #ccc;
	}

	/* Additional styles for white button with black text and rounded corners */
	.btn-white {
		background-color: white;
		border-color: white;
	}

	.btn-white:hover {
		background-color: #f0f0f0; /* Add a slight background color change on hover */
	}

	.btn-white.text-black {
		color: black;
	}

	.rounded-pill {
		border-radius: 50px; /* Adjust the border-radius value for the desired level of roundness */
	}

	/* Additional custom CSS for fine-tuning the design system */

	.card {
		border: none;
		transition: transform 0.3s;
	}

	.card:hover {
		transform: translateY(-5px);
	}

	.card-title {
		font-size: 1.5rem;
		font-weight: bold;
		color: #333;
	}

	.card-text {
		font-size: 1rem;
		color: #666;
	}

	.btn-purple {
		background-color: #663399;
		color: white;
	}

	.btn-purple:hover {
		background-color: darkpurple;
		color: white;
	}

	/* Navbar Toggle Icon Color */
	.navbar-toggler-icon {
		filter: invert(1);
	}
</style>
