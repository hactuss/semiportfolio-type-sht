<script>
    import ProjectCard from "$lib/components/ProjectCard.svelte";
    import FAQCard from "$lib/components/FAQCard.svelte";
    import ghlogo from "$lib/assets/images/github-mark-white.svg";
    import ss_spookymonth from "$lib/assets/images/Is it spooky month.png";
    import ss_ccenter from "$lib/assets/images/ccenter.png";
    import ss_Worldclock from "$lib/assets/images/Worldclock.png";
    let svelte_logo =
        "https://upload.wikimedia.org/wikipedia/commons/1/1b/Svelte_Logo.svg";
    let javascript_logo =
        "https://imgs.search.brave.com/2Lop95efMN3mNn8YORMHw4gXlmuiYbR1SXVpQQV4NCo/rs:fit:500:0:0:0/g:ce/aHR0cHM6Ly91cGxv/YWQud2lraW1lZGlh/Lm9yZy93aWtpcGVk/aWEvY29tbW9ucy90/aHVtYi85Lzk5L1Vu/b2ZmaWNpYWxfSmF2/YVNjcmlwdF9sb2dv/XzIuc3ZnLzI1MHB4/LVVub2ZmaWNpYWxf/SmF2YVNjcmlwdF9s/b2dvXzIuc3ZnLnBu/Zw";
    let screenshot = [ss_ccenter, ss_Worldclock, ss_spookymonth];
</script>

<main id="MAIN_CONTAINER">
    <main id="SIDEBAR">
        <!--
        <div id="SIDEBAR_LOGO">
            <img
                src="http://localhost:5173/src/lib/assets/haj-logo.svg"
                alt="haj-logo"
            />
            </div>-->
        <br />
        <span id="SIDEBAR_TEXT"> H A C T U S S</span>
        <br />
        <a href="https://github.com/hactuss">
            <img src={ghlogo} alt="github_logo" />
        </a>
    </main>
    <main id="MAIN_CONTENTS">
        <header>
            <h1>Name: <span class="marked">Hactuss</span></h1>
            <ul>
                <li>Frontend webdevelopment as a hobby</li>
                <li>
                    Primary programming language: <span id="marked2"
                        >Svelte</span
                    >
                </li>
                <li>Seeking job in IT industry</li>
            </ul>
        </header>
        <hr />
        <div id="Projects_wrapper">
            <h2>Projects</h2>

            <ProjectCard
                title="Center Calculator"
                buildtime="Sep 27. 2025"
                discription="A web app to automate the process of calculating the center of a given area. Useful in graphic design and more."
                url="https://center-calc.vercel.app"
            />
            <br />
            <ProjectCard
                title="Worldclock"
                buildtime="Dec 31. 2023"
                discription="a website to show the current time in different timezones. Useful when interacting with people from all around the world. (Currently being rewritten in svelte.)"
                url="https://hactuss.github.io/pages/office/office.html"
            />
            <br />
            <ProjectCard
                title="It is spooky month?"
                buildtime="Sep 15. 2025"
                discription="a small jokewebsite I built in reference to the Spooky Month indie animation series. Shows something special in october."
                url="https://isitspookymonth.vercel.app"
            />
        </div>
        <hr />
        <div>
            <h2>Personality</h2>
            <div>
                <h3>Hobbies</h3>
                <ul>
                    <li>Videoediting</li>
                    <li>Experimenting with Linux</li>
                    <li>Drawing comics</li>
                    <li>
                        Reading books regarding my hobbies or general literature
                    </li>
                    <li>Gaming</li>
                </ul>
            </div>
        </div>
        <hr />
        <footer>
            <p>
                Contact me via Email: <span class="marked"
                    >hactuss@proton.me</span
                >
            </p>
        </footer>
        {#if false}
            <div>
                <FAQCard
                    question="What does HAJ mean?"
                    answer="HAJ is an alias for domains that I use. For example, the website
                    uses this alias to shorten the URL. Otherwise, this would be unnecisarely
                    long if it was called hactuss-links.vercel.app.
                "
                />
            </div>
        {/if}
    </main>
</main>

<style>
    *::selection {
        color: rgb(50 50 50);
        background-color: rgb(200 250 20);
    }
    #SIDEBAR {
        width: 100%;
        flex: 1;
        display: flex;
        flex-direction: column;
        align-items: center;
        background-color: rgb(50, 50, 50);
    }
    #SIDEBAR_TEXT {
        writing-mode: vertical-lr;
    }
    #MAIN_CONTAINER {
        margin-left: 12.6%;
        margin-right: 12.6%;
        display: flex;
        height: 100%;
    }
    #MAIN_CONTENTS {
        width: 100%;
        display: flex;
        flex-direction: column;
    }

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
    /*#Projects_wrapper {
        border: solid 1px white;
        }*/
    img {
        width: 2.25rem;
    }

    .marked {
        color: rgb(200 250 20);
    }
    #marked2 {
        color: rgb(234 80 39);
    }
</style>
