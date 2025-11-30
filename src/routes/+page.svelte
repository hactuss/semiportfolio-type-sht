<script>
	import ProjectCard from '$lib/components/ProjectCard.svelte';
	import FAQCard from '$lib/components/FAQCard.svelte';
	import ghlogo from '$lib/assets/images/github-mark-white.svg';
</script>

<!--
<pre>
 ___  ___  ________  ________ _________  ___  ___  ________   ________
|\  \|\  \|\   __  \|\   ____\\___   ___\\  \|\  \|\   ____\ |\   ____\
 \ \  \\\  \ \  \|\  \ \  \___\|___ \  \_\ \  \\\  \ \  \___|_\ \  \___|_
  \ \   __  \ \   __  \ \  \       \ \  \ \ \  \\\  \ \_____  \\ \_____  \
   \ \  \ \  \ \  \ \  \ \  \____   \ \  \ \ \  \\\  \|____|\  \\|____|\  \
    \ \__\ \__\ \__\ \__\ \_______\  \ \__\ \ \_______\____\_\  \ ____\_\  \
     \|__|\|__|\|__|\|__|\|_______|   \|__|  \|_______|\_________\\_________\
                                                      \|_________\|_________|
</pre> -->

<main id="MAIN_CONTAINER">
	<main id="SIDEBAR">
		<!--
        <div id="SIDEBAR_LOGO">
            <img
                src="http://localhost:5173/src/lib/assets/haj-logo.svg"
                alt="haj-logo"
            />
            </div>-->
		<span id="SIDEBAR_TEXT">H A C T U S S</span>
		<div id="gh_link">
			<a href="https://github.com/hactuss" id="githublogo">
				<img src={ghlogo} alt="github_logo" />
			</a>
		</div>
	</main>
	<main id="MAIN_CONTENTS">
		<header>
			<h1>Name: <span id="marked1">Hactuss</span></h1>
			<ul>
				<li>Frontend webdevelopment as a hobby</li>
				<li>
					Primary programming language: <a id="marked2" href="https://svelte.dev/"
						>Svelte</a
					>
					and
					<a id="marked3" href="https://sass-lang.com/">SCSS</a>
				</li>
				<li>Seeking job in IT industry</li>
			</ul>
		</header>
		<hr />
		<div id="Projects_wrapper">
			<h2>Projects</h2>
			<ProjectCard
				title="Portfolio"
				buildtime="Nov 2. 2025"
				discription="This portfolio I created to tell about my projects and work."
				url="/"
				url_gh="https://github.com/hactuss/portfolio"
			/>
			<ProjectCard
				title="Center Calculator"
				buildtime="Sep 27. 2025"
				discription="A web app to automate the process of calculating the center of a given area. Useful in graphic design and more."
				url="https://center-calc.vercel.app"
				url_gh="https://github.com/hactuss/ccenter"
			/>
			<ProjectCard
				title="Worldclock"
				buildtime="Dec 31. 2023"
				discription="a website to show the current time in different timezones. Useful when interacting with people from all around the world. (Currently being rewritten in svelte.)"
				url="https://hactuss.github.io/pages/office/office.html"
				url_gh="https://github.com/hactuss/hactuss.github.io"
			/>
			<ProjectCard
				title="It is spooky month?"
				buildtime="Sep 15. 2025"
				discription="a small jokewebsite I built in reference to the Spooky Month indie animation series. Shows something special in october."
				url="https://isitspookymonth.vercel.app"
				url_gh="https://github.com/hactuss/isitspookymonthdotcom"
			/>
			<ProjectCard
				title="Ultrakill Terminal"
				buildtime="Nov 29. 2025"
				discription="a recreation of the terminals from the indiegame 'Ultrakill'"
				url="https://uk-terminal.vercel.app"
				url_gh="https://github.com/hactuss/uk-terminal"
			/>
		</div>
		<hr />
		<div>
			<h2>Personality</h2>
			<div>
				<h3>Hobbies</h3>
				<ul>
					<li>Videoediting</li>
					<li>
						Experimenting with Linux (Specifically <a
							id="marked4"
							href="https://nixos.org/">NixOS</a
						>)
					</li>
					<li>Drawing comics</li>
					<li>Reading books regarding my hobbies or general literature</li>
					<li>Gaming</li>
				</ul>
			</div>
		</div>
		<hr />
		<footer>
			<p>
				Contact me via Email: <span id="marked1">hactuss@proton.me</span>
			</p>
		</footer>
	</main>
</main>

<style>
	#SIDEBAR {
		flex: 1;
		display: flex;
		flex-direction: column;
		align-items: center;
		background-color: rgb(50, 50, 50);
	}
	#SIDEBAR_TEXT {
		writing-mode: vertical-lr;
		margin-top: 1rem;
		margin-bottom: 1rem;
	}
	#MAIN_CONTAINER {
		margin-left: 12.6%;
		margin-right: 12.6%;
		display: flex;
		flex-direction: row;
		height: 100%;
		backdrop-filter: brightness(0);

		filter: brightness(1);
	}
	#MAIN_CONTENTS {
		display: flex;
		flex-direction: column;
	}
	/*
    #SIDEBAR_LOGO {
        background-color: rgb(50 50 50);
        width: fit-content;
        height: fit-content;
        padding: 10px;
        border: transparent solid 1px;
        border-radius: 5px;
    }
    #SCREENSHOT_DISPLAY {
        opacity: 0.75;
        width: 400px;
    }
    #Projects_wrapper {
        border: solid 1px white;
    }*/
	img {
		width: 2.25rem;
	}
	span {
		margin: 0;
		padding: 0;
	}

	#marked1 {
		color: rgb(200 250 20);
	}
	#marked2 {
		color: rgb(234 80 39);
	}
	#marked3 {
		color: rgb(193 106 152);
	}
	#marked4 {
		color: rgb(82 107 171);
	}

	@media screen and (width <= 500px) {
		#MAIN_CONTAINER {
			flex-direction: column;
			margin: 0;
		}
		#SIDEBAR {
			display: flex;
			flex-direction: row;
			align-items: flex-end;
			justify-content: space-between;
		}
		#SIDEBAR_TEXT {
			writing-mode: horizontal-tb;
			margin-left: 1rem;
		}
	}
	#sv {
		position: absolute;
		top: 300px;
	}
</style>
