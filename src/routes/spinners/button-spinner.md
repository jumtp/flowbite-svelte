---
layout: doc
---

<script>
  import { SpinnerButton }from '$lib/index';
</script>


<h1 class="text-3xl w-full dark:text-white py-8">Button spinner</h1>


```svelte
<script>
  import { SpinnerButton } from "flowbite-svelte";
</script>
```

<h2 class="text-2xl mt-8 dark:text-white py-8">Default Prop</h2>

```js
let color; // 'blue' | undefined
```

<h2 class="text-2xl mt-8 dark:text-white py-8">Colors</h2>

<div class="container w-full rounded-xl my-4 mx-auto bg-gradient-to-r bg-white dark:bg-gray-900 border border-gray-200 dark:border-gray-700 p-2 sm:p-6">
<SpinnerButton />
<SpinnerButton color="blue" />
</div>

```svelte
<SpinnerButton />
<SpinnerButton color="blue" />
```

<h2 class="text-2xl mt-8 dark:text-white py-8">Slot</h2>

<div class="container w-full rounded-xl my-4 mx-auto bg-gradient-to-r bg-white dark:bg-gray-900 border border-gray-200 dark:border-gray-700 p-2 sm:p-6">
<SpinnerButton>Here you go ...</SpinnerButton>
<SpinnerButton color="blue" >Here you go ...</SpinnerButton>
</div>

```svelte
<SpinnerButton>Here you go ...</SpinnerButton>
<SpinnerButton color="blue" >Here you go ...</SpinnerButton>
```

<h2 class="text-2xl w-full dark:text-white py-8">Related components</h2>

<p class="dark:text-white text-lg w-full"><a href="https://flowbite-svelte.vercel.app/spinners/default" class="text-blue-600 hover:underline dark:text-blue-500">Default Spinner</a></p>

<p class="dark:text-white text-lg w-full"><a href="https://flowbite-svelte.vercel.app/spinners/button-spinner" class="text-blue-600 hover:underline dark:text-blue-500">Button Spinner</a></p>

<h2 class="text-2xl w-full dark:text-white py-8">References</h2>

<p class="dark:text-white text-lg"><a href="https://flowbite.com/docs/components/spinner/" target="_blank" class="text-blue-600 hover:underline dark:text-blue-500">Flowbite Spinner</a></p>