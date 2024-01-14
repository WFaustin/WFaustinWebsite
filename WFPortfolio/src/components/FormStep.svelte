<script>
    export let step; 
</script>

<form action="https://formspree.io/f/mrgnbkpw" method="POST" class="p-4 sm:p-6 md:p-8 flex flex-col
gap-4 rounded-lg border border-solid border-violet-700 text-center group
cursor-pointer hover:border-violet-400 duration-200">

    <div class="bg-slate-950 grid place-items-center px-4 text-5xl md:text-6xl 
    -mt-10 sm:-mt012 md:-mt-14 lg:-mt-16 mx-auto duration-200">
        <img src={step.icon} alt={step.name + ' Logo'} class="flex object-scale-down mx-auto step-img" />

    </div>
    <h3 class="font-medium text-xl sm:text-xl md:text-2xl">{step.name}</h3>
    <slot/>
    <!-- Replace with accesKey sent to your email -->
    <input type="hidden" name="accessKey" value="449ab33e-e7c1-401e-b6ce-a8cba74307c0"> <!-- Required -->
    <input type="text" name="name" placeholder="Your Name" class="text-black"> <!-- Optional -->
    <input type="text" name="subject" placeholder="Your Subject" class="text-black"> <!-- Optional -->
    <input type="text" name="email" placeholder="Your Email" class="text-black"> <!-- Optional -->
    <textarea name="message" class="text-black"></textarea> <!-- Optional -->
    <!-- Specify @ as reply to value if you want it to be customers email -->
    <input type="hidden" name="replyTo" value="@"> <!-- Optional -->
    <!-- If you want form to redirect to a specific url after submission -->
    <input type="hidden" name="redirectTo" value="/"> <!-- Optional -->
    <input type="text" name="honeypot" style="display: none;"> <!-- Optional -->
    <!--End of Comments-->
    <div class="flex-1 flex justify-between gap-4 items-center">
        <div class="ml-auto cursor-pointer hover:text-slate-950 duration-200
        relative after:absolute after:top-0 after:h-0 after:right-full after:w-full
        after:h-full after:bg-white after:duration-200 hover:after:translate-x-full after:z-[-1]
        overflow-hidden">
            <input type="submit" class="relative z-4" value='&rarr;' />
        </div>
    </div>
</form>