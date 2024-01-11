<script>
    import Step from "../../components/Step.svelte";

    let steps = [
        {name: 'Linkedin', icon: 'assets/linkedin-logo-3.png'}, 
        {name: 'Email', icon: 'assets/Email-Logo-PNG.png'}
    ];
</script>

<div>
    <h2>Contact Me</h2>
    <br/>
    <h4>Here's Some Ways To Get In Touch With Me:</h4>
</div>

<div>
    <Step step={steps[0]}>
    
    </Step>
    <Step step={steps[1]}>
    
    </Step>
</div>