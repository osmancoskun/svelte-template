<script>
    import { metatags } from '@roxi/routify'
    import Button from "../components/m-button.svelte"
    
    metatags.title = 'Svelte Template'
    metatags.description = 'Svelte Template with Beautiful Components'
</script>

<h1>Svelte Template With Components</h1>

<Button disabled={true} textColor="blue" radius="10px" border="2px" borderInPx="2px" borderColor="green" shadow={true} >Osman</Button>
<Button>
    Normal Button
</Button>
<Button borderInPx="2px" borderColor="gray">Button With Border</Button>
<Button borderInPx="2px" borderColor="Violet">Button With Violet Border</Button>
<Button borderInPx="2px" borderColor="gray" textColor="blue">Button With Blue Text</Button>

<Button borderInPx="2px" borderColor="gray" radius="10px">Button With 10px Radius</Button>



