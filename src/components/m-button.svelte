<script>
    export let id
    export let color
    export let textColor
    export let borderColor
    export let borderInPx
    export let radius
    export let disabled
    export let shadow

    let node
    if(node){
        
    }
</script>
<button {disabled} {id} on:click bind:this={node} style="--color:{color};--text-color:{textColor};
--radius:{radius};--border:{borderInPx};--border-color:{borderColor};--shadow:{shadow ? '0 0px 0px 0 rgba(0,0,0,0.24), 0 5px 5px 0 rgba(0,0,0,0.19)' : 0}">
    <slot/>
</button>

<style>

button{
background-color: var(--color);
color:var(--text-color);
border-radius: var(--radius);
border:var(--border) solid var(--border-color);
}
button:hover{
    box-shadow: var(--shadow);
}

</style>