<script>
    import { Meta, Template, Story } from "@storybook/addon-svelte-csf";
    import Button from "../lib/Button.svelte";
</script>

<Meta
        title="Yolo/Button"
        component={Button}
        argTypes={{
      color: { control: "color" },
    }}
/>

<Template let:args>
    <Button {...args} on:click={args.onClick} />
</Template>


<Story
        name="Red"
        args={{
      color: "red",
    }}
/>


<Story
        name="Blue"
        args={{
      color: "blue",
    }}
/>
