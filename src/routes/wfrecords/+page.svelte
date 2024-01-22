<script>

let benefits = [
        {name: 'An Audio Initiative:', description: "Used to cultivate my passion for creating and composing, "
        + "WFRecords aims to combine passion with career in multiple ways, focusing on the creation of music/sound "
        + "to be incorporated in games, videos, and streaming."},
        {name: 'A Music Alternative for Smaller Creators:', description: "With the amount of online creators that have emerged in the past 2 decades, "
        + "it can be incredibly difficult to differentiate yourself from the rest of the crowd. One way smaller creators can enhance their products is through music, "
        + "but the cost of getting custom music often is too much to justify. WFRecords aims to help remedy this issue and gives creators a more cost-effective avenue "
        + "to unique music, without having to settle for royalty-free tunes."},
    ];

</script>


<section class="py-20 lg:py-32 flex flex-col gap-24">
    <div class="flex flex-col gap-2 text-center">
        <h1 class="font-bold text-4xl sm:text-6xl md:text-7xl">
            <span class="text-violet-400">WFRecords</span>
        </h1>
        <br/>
    </div>
</section>
<section id="about" class="py-20 pt-10 lg:pt-16 lg:py-32 flex flex-col gap-16 sm:gap-20 md:gap-24 relative">
    <div class="flex flex-col gap-2 text-center relative before:absolute before:top-0 before:left-0
    before:w-2/3 before:h-1.5 before:bg-violet-700 after:absolute after:bottom-0 after:right-0
    after:w-2/3 after:h-1.5 after:bg-violet-700 py-4">
    <h3 class="font-semi-bold text-3xl sm:text-4xl md:text-5xl">
        What is <span class="text-violet-400">WFRecords</span>?
        <br/>
    </h3>
    </div>
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
        <div class="blueShadow relative overflow-hidden px-5 py-2 group rounded-full bg-white
        text-slate-950">
            <a href="https://wfaustin.github.io/WFRecordings/" target="_blank" class="pointer-events-none cursor-default">
                <div class="relative top-0 right-0 w-1 h-full bg-violet-400 opacity-20
                group-hover:translate -x-half z-0 duration-200">

                </div>
                <h4 class="relative z-9 text-center">Visit WFRecordings</h4>
            </a>
        </div>
        <p>*Note - WFRecordings is currently under construction, and as such the link may not be accessible.</p>
    </div>
</section>