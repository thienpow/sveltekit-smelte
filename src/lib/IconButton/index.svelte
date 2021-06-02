<script>
  import Button from "smelte/src/components/Button"

  export let value = false
  export let icon = null
  export let color = null
  export let iconClass = "flex items-center select-none p-2"
</script>
  
<div on:mouseleave>
  <Button icon={icon} flat text
    {color} {iconClass}
    add="{color ? color : 'dark:text-white text-primary-a700'}" remove="py-2 px-4 p-4" 
    on:click={() => (value = !value)}
    on:click
    on:mouseover
    on:*
  />
</div>