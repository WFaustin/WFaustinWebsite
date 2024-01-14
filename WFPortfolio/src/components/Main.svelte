<script>
    import Step from "./Step.svelte";

    let steps = [
        {name: 'Dayfarers', icon: 'assets/PDF_LOGO_White_Small.png', href: 'https://cosmic-engine.gitlab.io/'},
        {name: 'Chess Validation', icon: 'assets/Chess_rdt60.png', href: 'https://gitlab.com/WFaustin/chessvalidationprojectse576'},
        {name: 'Toast', icon: 'assets/Group 399.png', href: 'https://github.com/Salud-Team/SaludDevelopment'} 
    ];

    let benefits = [
        {name: 'a motivated developer:', description: "With a Bachelor\'s and " +
        "Master\'s degree in Computer Science, I have had the opportunity to work on some impressive" +
        " and innovative projects. I love when opportunities to make cool stuff graces my doorstep," + 
        " and I try to take any and every opportunity to learn something new in the space."},
        {name: 'an creative soul:', description: 'Whether it comes to my career or my freetime, I love' +
        ' being able to use my creativity to solve problems and create beautiful things. As a musician, I\'ve learned '
        + 'that there rarely is just one way to get to the destination you want to arrive at, and that sort '
        + ' of flexiblity has gotten me out of some difficult artist\'s block.'},
        {name: 'a collaborative leader:', description: 'One thing that I\'ve learned so far in my career is how beneficial'
        + ' it is to work with those with different skillsets and experiences. Being able to learn from others while also'
        + ' displaying the expertise that you have gained makes working together both enriching and successful. In that way,'
        + ' even if all of us aren\'t designated as a \'leader\' in every single project, we can all bring leadership in our own way.'}
    ];
</script>
<main class="flex flex-col flex-1 p-4">
    <section id="introPage" class="grid grid-cols-1 lg:grid-cols-2 gap-10 py-8 sm:py-14">
        <div class="flex flex-col lg:justify-center text-center lg:text-center gap-6 md:gap-8
        lg:gap-10">
            <h2 class="font-semibold text-4xl sm:text-5xl md:text-6xl">
                <span class="poppins text-violet-400"> Widchard </span> Faustin
            </h2>
            <h3 class="font-semibold text-2xl sm:text-3xl md:text-3xl">
                <br/> Full Stack <span class="poppins text-violet-400">Developer</span>
                <br/> Game <span class="poppins text-violet-400">Programmer</span>
                <br/> Musician | <span class="poppins text-violet-400">Composer</span>
                <br/> Sound <span class="poppins text-violet-400">Designer</span>
            </h3>
            <p class="text-base sm:text-lg md:text-xl">
                Some of my <span class="text-violet-400">favorite</span> languages/frameworks are Python, C#, Node.JS, SvelteJS, and Godot.
            </p>
        </div>
        <div class="relative shadow-2xl grid place-items-center opacity-100">
            <img src={"assets/WidchardWeb.png"} alt="Profile Image" class="object-cover z-[2] max-w-[45vw] max-h-[70vh]"/>
        </div>
    </section>
    <section class="py-20 lg:py-32 flex flex-col gap-24" id="projects">
        <div class="flex flex-col gap-2 text-center">
            <h3 class="font-semi-bold text-3xl sm:text-4xl md:text-5xl">
                Some of my <span class="text-violet-400">technical work</span> on display.
            </h3>
        </div>
        <div class="grid justify-center grid-cols-1 lg:grid-cols-3 gap-12 lg:gap-10">
            <Step step={steps[0]}>
                <p>Dayfarers was an award winning senior capstone project developed in 2021.
                 A turn-based RPG where the player has to use the time-travel mechanics against
                 adversaries to turn the tables and be victorious, Dayfarer was the most
                 ambitious group project of my academic career, both as a programmer and a composer. 
                 <br/> Created with <strong class='text-violet-400'>Godot + GDScript</strong>.
                </p>
            </Step>
            <Step step={steps[1]}>
                <p>The Chess Validation Project was a course project that not only tested student's 
                skills in coding, but also their proficiency in testing and validation, especially 
                against edge cases. This project was a great way to freshen up our coding skills
                along with teaching us how to be thorough in testing.
                <br/> Created with <strong class='text-violet-400'>Java</strong>.
                </p>
            </Step>
            <Step step={steps[2]}>
                <p> One of my first dips into Full-Stack Development, Toast was a case of being a sole
                developer being asked to create a web application and having no idea where to start. 
                An application whose goal was to be able to send food and drinks to others as gifts ("Toasts"), 
                this project tested my current knowledge as well as gave me new skills.
                <br/> Created with <strong class='text-violet-400'>Angular.JS + Node.JS + MongoDB</strong>.
                </p>
            </Step>
        </div>
    </section>
    <section id="about" class="py-20 pt-10 lg:pt-16 lg:py-32 flex flex-col gap-16 sm:gap-20 md:gap-24 relative">
        <div class="flex flex-col gap-2 text-center relative before:absolute before:top-0 before:left-0
        before:w-2/3 before:h-1.5 before:bg-violet-700 after:absolute after:bottom-0 after:right-0
        after:w-2/3 after:h-1.5 after:bg-violet-700 py-4">
            <h3 class="font-semibold text-3xl sm:text-4xl md:texl-5xl">
                Some Facts <span class="poppins text-violet-400">About Me</span>
            </h3>
        </div>
        <p class="mx-auto poppins font-semibold text-lg sm:text-xl md:text-2xl"> I am . . .</p>
        <div class="flex flex-col gap-20 w-full mx-auto max-w-[800px]">
            {#each benefits as benefit, index}
                <div class="flex gap-6 sm:gap-8">
                    <div class="flex gap-6 sm:gap-8">
                        <p class="poppins text-4xl sm:text-5xl md:text-6xl text-slate-500 
                        font-semibold">
                            0{index+1}
                        </p>
                        <div class="flex flex-col gap-6 sm:gap-8">
                            <h3 class="text-2xl sm:text-3xl md:text-5xl">
                                {benefit.name}
                            </h3>
                            <p>{benefit.description}</p>
                        </div>
                    </div>
                </div>
            {/each}
        </div>
    </section>
</main>

