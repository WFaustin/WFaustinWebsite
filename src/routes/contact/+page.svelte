<script>
    import Step from "../../components/Step.svelte";
    import FormStep from "../../components/FormStep.svelte";
    import DownloadStep from "../../components/DownloadStep.svelte";

    let steps = [
        {name: 'Linkedin', icon: 'assets/linkedin-logo-3.png', href: 'https://www.linkedin.com/in/w-f-275chs/'}, 
        {name: 'Github', icon: 'assets/github.png', href: 'https://github.com/WFaustin'},
        {name: 'Email', icon: 'assets/Email-Logo-PNG.png'},
        {name: 'Resume', icon: 'assets/resume-icon.png'},
    ];
</script>

<section class="py-20 lg:py-32 flex flex-col gap-24">
    <div class="flex flex-col gap-2 text-center">
        <h2 class="font-bold text-4xl sm:text-6xl md:text-7xl">
            <span class="text-violet-400">Contact Me</span>
        </h2>
        <br/>
        <br/>
        <br/>
    </div>
</section>
<section class="py-20 lg:py-32 flex flex-col gap-24">
    <div class="flex flex-col gap-2 text-center">
        <h3 class="font-semi-bold text-3xl sm:text-4xl md:text-5xl">
            Here's Some Ways To <span class="text-violet-400">Get In Touch</span> With Me.
            <br/>
        </h3>
    </div>
</section>
<section class="py-20 lg:py-32 flex flex-col gap-24">
    <div class="grid justify-center grid-cols-1 lg:grid-cols-2 gap-12 lg:gap-10">
        <Step step={steps[0]}>
            <p>
                For those who'd like to connect with me on <strong class='text-violet-400'>Linkedin</strong>.
                <br/>
                <br/>
                <br/>
                <br/>
                <br/>
                <br/>
                <br/>
                <br/>
            </p>
        </Step>
        <Step step={steps[1]}>
            <p>
                For those who'd like to check out some of my projects on <strong class='text-violet-400'>Github</strong>.
                <br/>
                <br/>
                <br/>
                <br/>
                <br/>
                <br/>
                <br/>
                <br/>
            </p>
        </Step>
        <FormStep step={steps[2]}>
            <p> 
                For those who'd like to directly send me an <strong class='text-violet-400'>email</strong>.
            </p>
        </FormStep>
        <DownloadStep step={steps[3]}>
            <p> 
                For those who'd like to see my <strong class='text-violet-400'>resume</strong>.
            </p>
            <div>

            </div>
        </DownloadStep>
    </div>
</section>
