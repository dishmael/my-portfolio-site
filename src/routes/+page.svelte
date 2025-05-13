<script lang="ts">
	import ExperienceCard from '$lib/components/ExperienceCard.svelte';
	import Footer from '$lib/components/Footer.svelte';
	import GithubIcon from '$lib/components/GithubIcon.svelte';
	import Hero from '$lib/components/Hero.svelte';
	import LinkedInIcon from '$lib/components/LinkedInIcon.svelte';
	import Navlink from '$lib/components/Navlink.svelte';
	import ProjectCard from '$lib/components/ProjectCard.svelte';
</script>

<div class="mx-auto min-h-screen max-w-screen-xl px-6 py-12 font-sans md:px-12 md:py-16 lg:py-0">
	<div class="lg:flex lg:justify-between lg:gap-4">
		<header
			class="lg:sticky lg:top-0 lg:flex lg:max-h-screen lg:w-[48%] lg:flex-col lg:justify-between lg:py-24"
		>
			<Hero />
			<nav class="nav hidden lg:mt-10 lg:block">
				<ul class="w-max">
					<Navlink title="About" href="#about" />
					<Navlink title="Experience" href="#experience" />
					<Navlink title="Projects and Experiments" href="#projects" />
				</ul>
			</nav>
			<ul class="mt-8 mb-8 ml-1 flex items-center md:mb-12 lg:mt-auto lg:mb-0">
				<GithubIcon />
				<LinkedInIcon />
			</ul>
		</header>

		<main id="content" class="lg:w-[52%] lg:py-24">
			<!-- ABOUT -->
			<section
				id="about"
				class="scroll-mt-16 sm:mb-4 md:mb-12 lg:mb-16 lg:scroll-mt-24"
				aria-label="About me"
			>
				<div
					class="sticky top-0 z-20 -mx-6 mb-4 w-screen bg-slate-900/75 px-6 py-5 backdrop-blur md:-mx-12 md:px-12 lg:sr-only lg:relative lg:top-auto lg:mx-auto lg:w-full lg:px-0 lg:py-0 lg:opacity-0"
				>
					<h2 class="text-sm font-bold tracking-widest text-slate-200 uppercase lg:sr-only">
						About
					</h2>
				</div>
				<div>
					<p class="mb-4">
						With more than 25 years of experience in technology-driven environments, I specialize in
						leading engineering teams, driving innovation, and optimizing operations for business
						success. My career has been defined by strategic leadership, managing cross-functional
						teams, and spearheading projects that enhance efficiency and customer satisfaction. From
						building multi-million-dollar revenue pipelines to expanding service offerings, I thrive
						on solving complex challenges through forward-thinking solutions.
					</p>

					<p class="mb-4">
						My expertise spans <strong
							>software engineering, cloud computing, database administration, data engineering and
							analytics, system administration, enterprise architecture, and service delivery</strong
						>, utilizing technologies programming languages such as Docker, Python, React,
						TypeScript, and Golang. Whether leading teams or crafting solutions that elevate
						performance, I focus on fostering collaboration and continuous improvement. I take pride
						in mentoring talent, ensuring teams are equipped to meet evolving industry demands and
						deliver impactful results.
					</p>

					<p class="mb-4">
						I am passionate about innovation and problem-solving. I am always exploring new ways to
						drive measurable business outcomes. My leadership philosophy emphasizes adaptability,
						customer-centric strategies, and technology-driven insights to fuel success.
					</p>
				</div>
			</section>

			<!-- EXPERIENCE -->
			<section
				id="experience"
				class="mb-16 scroll-mt-16 md:mb-24 lg:mb-36 lg:scroll-mt-24"
				aria-label="Work experience"
			>
				<div
					class="sticky top-0 z-20 -mx-6 mb-4 w-screen bg-slate-900/75 px-6 py-5 backdrop-blur md:-mx-12 md:px-12 lg:sr-only lg:relative lg:top-auto lg:mx-auto lg:w-full lg:px-0 lg:py-0 lg:opacity-0"
				>
					<h2 class="text-sm font-bold tracking-widest text-slate-200 uppercase lg:sr-only">
						Experience
					</h2>
				</div>
				<div>
					<ol class="group/list">
						<ExperienceCard heading="Vice President, Qmulos" from="2023" to="2025" skills={[]}>
							<p class="mt-2 text-sm leading-normal">
								Provided leadership for the delivery team, with a strong emphasis on engineering
								excellence and operational efficiency. Led a team of 40+ skilled directors, managers,
								and engineers, overseeing technical execution, project delivery, and continuous
								improvement of engineering best practices. Spearheaded initiatives to enhance
								engineering team health, optimize workflows, and align technical efforts with
								corporate-level objectives. Fostered a customer-centric and innovation-driven
								culture while ensuring resource utilization, profitability, and cross-functional
								collaboration between engineers, partners, customers, and the product organization.
								Played a critical role in business development, leveraging technical expertise to
								expand service offerings and drive sustainable growth.
							</p>
						</ExperienceCard>
						<ExperienceCard
							heading="Managing Director, Stratascale"
							from="2022"
							to="2023"
							skills={[]}
						>
							<p class="mt-2 text-sm leading-normal">
								Managed the Data and Analytics team, driving engineering excellence in data-centric
								solutions and service delivery. Managed a team of directors, and engineers,
								analysts, and scientists, overseeing the design, development, and delivery of
								cutting-edge analytics platforms and AI-driven insights. Established engineering
								best practices, optimized technical workflows, and fostered a high-performing,
								innovation-driven environment. Provided strategic guidance and mentorship to
								engineers, ensuring alignment with business objectives and technical advancements.
								Spearheaded efforts to expand service offerings and leverage emerging technologies
								to enhance data-driven decision-making.
							</p>
						</ExperienceCard>
						<ExperienceCard heading="Vice President, Trace3" from="2017" to="2021" skills={[]}>
							<p class="mt-2 text-sm leading-normal">
								Developed and grew the Intelligent Operations practice with a strong focus on Site
								Reliability Engineering (SRE), Observability, and AIOps. Managed a distributed team
								of directors and engineers, overseeing the design, deployment, and optimization of
								scalable, high-performance systems. Crafted and implemented reference architectures
								to enhance client environments, driving reliability, automation, and operational
								efficiency. Provided strategic technical leadership, aligning engineering efforts
								with business objectives while fostering an innovation-driven culture. Spearheaded
								business development initiatives to expand service offerings and integrate
								cutting-edge technologies for improved observability and incident response
							</p>
						</ExperienceCard>
						<ExperienceCard
							heading="Chief Technology Officer, OpsVision Solutions"
							from="2013"
							to="2017"
							skills={[]}
						>
							<p class="mt-2 text-sm leading-normal">
								Developed and grew the Intelligent Operations practice with a strong focus on Site
								Reliability Engineering (SRE), Observability, and AIOps. Managed a distributed team
								of directors and engineers, overseeing the design, deployment, and optimization of
								scalable, high-performance systems. Crafted and implemented reference architectures
								to enhance client environments, driving reliability, automation, and operational
								efficiency. Provided strategic technical leadership, aligning engineering efforts
								with business objectives while fostering an innovation-driven culture. Spearheaded
								business development initiatives to expand service offerings and integrate
								cutting-edge technologies for improved observability and incident response.
							</p>
						</ExperienceCard>
						<ExperienceCard
							heading="Sr. Enterprise Architect & Software Developer, SMS Data Products"
							from="2010"
							to="2013"
							skills={[]}
						>
							<p class="mt-2 text-sm leading-normal">
								As Senior Enterprise Architect and Software Developer for a technology consulting
								firm, my responsibilities were critical to the success of our clients' digital
								transformation journeys. I was entrusted with envisioning and designing
								comprehensive enterprise-level architectures that align with business objectives and
								leverage cutting-edge technologies. I collaborated closely with clients to
								understand their unique needs, challenges, and goals, and translated them into
								robust and scalable architectural solutions. I lead a team of talented architects
								and guided them in developing strategic roadmaps, blueprints, and implementation
								plans that optimize technology investments and drove innovation.
							</p>
						</ExperienceCard>
						<ExperienceCard
							heading="Sr. Engineer & Software Developer, SMS Data Products"
							from="2000"
							to="2010"
							skills={[]}
						>
							<p class="mt-2 text-sm leading-normal">
								Holding multiple roles to include Senior Engineer, Software Developer, and IT
								Director for a technology consulting firm, my responsibilities encompassed a wide
								range of crucial tasks. Leading a team of engineers, analysts, and technicians, I
								oversaw the design, development, and implementation of innovative technology
								solutions for our clients. I collaborated closely with clients to understand their
								business needs and translate them into effective technical strategies. Managing the
								IT infrastructure, I ensured its stability, security, and scalability, while also
								identifying opportunities for optimization and enhancement.
							</p>
						</ExperienceCard>
					</ol>
				</div>
			</section>

			<!-- PROJECTS -->
			<section
				id="projects"
				class="mb-16 scroll-mt-16 md:mb-24 lg:mb-36 lg:scroll-mt-24"
				aria-label="projects and experiments"
			>
				<div
					class="sticky top-0 z-20 -mx-6 mb-4 w-screen bg-slate-900/75 px-6 py-5 backdrop-blur md:-mx-12 md:px-12 lg:sr-only lg:relative lg:top-auto lg:mx-auto lg:w-full lg:px-0 lg:py-0 lg:opacity-0"
				>
					<h2 class="text-sm font-bold tracking-widest text-slate-200 uppercase lg:sr-only">
						Projects and Experiments
					</h2>
				</div>
				<p>This area is a Work in Progress</p>
				<ProjectCard
					heading="This Portfolio Site"
					imgSrc="/images/portfolio-site.png"
					skills={['Svelte 5', 'Tailwind CSS', 'Railway', 'Cloudflare']}
				>
					<p>
						I typically work with React and TypeScript, but I wanted to ramp up on Svelte to see
						what all the fuss was about. So what better way to learn than to create a new portfolio
						site. This is a WIP and I will likely add more features over time.
					</p>
				</ProjectCard>
				<ProjectCard
					heading="Screen Capture API"
					imgSrc="/images/nestjs-screen-capture.png"
					skills={['NestJS', 'Puppeteer', 'Swagger']}
				>
					<p>
						This is part of a feature for a larger MVP that is still being developed. The API is
						used to fetch a live screen capture of a remote URL and deliver the image as a base64
						string to be used by the calling client.
					</p>
				</ProjectCard>
				<ProjectCard
					heading="Snap-Telemetry"
					imgSrc="/images/snap-telemetry.png"
					skills={['Golang', 'AWS SQS', 'SignalFx', 'Syslog']}
				>
					<p>
						I was a contributor to Snap Telemetry (Snap), an open telemetry framework designed to
						simplify the collection, processing and publishing of system data through a single API.
					</p>
				</ProjectCard>
				<ProjectCard
					heading="Old Portfolio Site"
					imgSrc="/images/old-portfolio-site.png"
					skills={['Wix']}
				>
					<p>
						My original portfolio site was built on Wix. It was a great way to get started, but it
						did not showcase my development skills.
					</p>
				</ProjectCard>
			</section>
		</main>
	</div>
	<Footer />
</div>
