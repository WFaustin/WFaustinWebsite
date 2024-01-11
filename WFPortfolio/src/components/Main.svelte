<script>
    import Step from "./Step.svelte";

    let steps = [
        {name: 'Dayfarers', icon: 'assets/PDF_LOGO_White_Small.png'},
        {name: 'Chess Validation', icon: 'assets/Chess_rdt60.png'},
        {name: 'Toast', icon: 'assets/Group 399.png'} 
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
                <br/> Audio <span class="poppins text-violet-400">Engineer</span>
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
                Some of my <span class="text-violet-400">work</span> on display.
            </h3>
        </div>
        <div class="grid justify-center grid-cols-1 lg:grid-cols-3 gap-12 lg:gap-10">
            <Step step={steps[0]}>
             
            </Step>
            <Step step={steps[1]}>
             
            </Step>
            <Step step={steps[2]}>
             
            </Step>
        </div>
    </section>
</main>

