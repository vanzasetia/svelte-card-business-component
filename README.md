# Card Business Component with Svelte

This is my first project with Svelte. It is a static website.

The purpose of doing this project is to get familiar with Svelte.

[Card Business Component with Svelte](https://svelte-laurasmithbusiness.netlify.app/)

## Built with

- [Svelte • Cybernetically enhanced web apps](https://svelte.dev/)
- HTML Semantic Tags
- [BEM (Block, Element, Modifier)](https://sparkbox.com/foundry/bem_by_example)
- CSS Flexbox
- Mobile-first workflow

## What I learned

I learned the very basics of Svelte.

### Create Svelte components

I learned to separate HTML and very little CSS into Svelte components.

Svelte uses standard HTML markup such as `<script>` and `<style>` which makes it easy to get started. Also, it does not look scary.

Svelte component can also be as simple as the following:

```svelte
<!-- Heading.svelte -->
<h1>Hello world!</h1>
```

To use the `Heading` component, I can do the following:

```svelte
<!-- App.svelte -->
<script>
  import Heading from "./Heading.svelte";
</script>

<Heading />
```

### How to have a dynamic component inside a component?

I wonder if it is possible to have a custom nested element. For example, I want to have a `Button` component that can have a different icon. Then, the icon should be an inline SVG

```svelte
<!-- Button.svelte -->
<script>
  export let icon;
</script>

<button type="button">
  {icon}
</button>
```

My question is how to add an inline SVG to the `Button` component?

I tried this and it didn't work:

```svelte
<!-- App.svelte -->
<script>
  import Button from "./Button.svelte";
</script>

<Button icon={<svg xmlns="http://www.w3.org/2000/svg" width="24" height="28" viewBox="0 0 24 28"><path d="M19.5 2C21.984 2 24 4.016 24 6.5v15c0 2.484-2.016 4.5-4.5 4.5h-2.938v-9.297h3.109l.469-3.625h-3.578v-2.312c0-1.047.281-1.75 1.797-1.75L20.265 9V5.766c-.328-.047-1.469-.141-2.781-.141-2.766 0-4.672 1.687-4.672 4.781v2.672H9.687v3.625h3.125V26H4.499a4.502 4.502 0 0 1-4.5-4.5v-15c0-2.484 2.016-4.5 4.5-4.5h15z"/></svg>} />
```

I can't use `@html` either.

So, my solution for this problem was to convert SVGs into Svelte components.

## Useful resources

- [Docs • Svelte](https://svelte.dev/docs) - This can be a handy page when I want to learn and remind something about Svelte.
- [Svelte Tutorial](https://svelte.dev/tutorial/) - This helped me learn the basics of Svelte.
- [Svelte Examples](https://svelte.dev/examples/styling) - This can be a great page to see Svelte code in action.

## License

[MIT](./LICENSE)
