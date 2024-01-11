<script>
    export let step; 
</script>

<a href={step.href} target="_blank" class="p-4 sm:p-6 md:p-8 flex flex-col
gap-4 rounded-lg border border-solid border-violet-700 text-center group
cursor-pointer hover:border-violet-400 duration-200">
    <div class="bg-slate-950 grid place-items-center px-4 text-5xl md:text-6xl 
    -mt-10 sm:-mt012 md:-mt-14 lg:-mt-16 mx-auto duration-200">
        <img src={step.icon} alt={step.name + ' Logo'} class="flex object-scale-down mx-auto h-50px w-50px step-img" />

    </div>
    <h3>{step.name}</h3>
    <slot/>
    <div>
        <div>
            <p class="relative z-4">Go to &rarr;</p>
        </div>
    </div>
</a>