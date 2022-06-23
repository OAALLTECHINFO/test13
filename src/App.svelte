<script>
  import { ComboBox } from "fluent-svelte";
</script>

<style>
	@import url("https://unpkg.com/fluent-svelte/theme.css");

	/* Some base styles to get things looking right. */
	:global(body) {
		background-color: var(--fds-solid-background-base);
		color: var(--fds-text-primary);
	}
</style>

<h2>
	Hello Guys
</h2>
<h2>
	Welcom to The OA
</h2>
<main>
  hello
  <ComboBox
		scroll-behavior: auto
    value="6"
    items={Array.from(Array(50).keys()).map((i) => ({
      name: `Item ${i}`,
      value: i.toString(),
    }))} />
</main>