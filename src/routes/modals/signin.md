---
layout: doc
---

<script>
  import { SignInModal, ModalButton, modalIdStore }from '$lib/index';

  const closeModal = () => {
    modalIdStore.update((value) => {
      value = null;
    });
  };

  let signinId = "signin-modal2";
  let btnSignInName = "Sign In Modal";
  let btnSignInColor = "blue";
</script>

<h1 class="text-3xl w-full dark:text-white py-8">Sign-in Modals</h1>

<h2 class="text-2xl w-full dark:text-white py-8">Set up</h2>

<p class="dark:text-white text-base py-4">Import SignInModal, ModalButton components and set variables in the script tag.</p>

```svelte
import { SignInModal, ModalButton, modalIdStore } from "flowbite-svelte";

let signinId = "signin-modal2";
let btnSignInName = "Sign In Modal";
let btnSignInColor = "blue";
```

<h2 class="text-2xl w-full dark:text-white py-8">SignIn Modals</h2>

<div class="container flex flex-wrap justify-center rounded-xl mx-auto bg-gradient-to-r bg-white dark:bg-gray-900 border border-gray-200 dark:border-gray-700 p-2 sm:p-6">
  <ModalButton
    id={signinId}
    btnName={btnSignInName}
    btnColor={btnSignInColor}
  />
</div>

<p class="dark:text-white text-base py-4">Create a button and modal.</p>

```svelte
<ModalButton
  id={signinId}
  btnName={btnSignInName}
  btnColor={btnSignInColor}
/>
<SignInModal
  id={signinId}
  titleSignIn=SignIn Modal Title"
  lostPasswordLink="/auth/lost-password"
  signUpLink="/auth/signup"
  formLink="/auth/signin"
/>
```

<SignInModal
  id={signinId}
  titleSignIn="SignIn Modal Title"
  lostPasswordLink="/"
  signUpLink="/about"
  formLink="/modals"
/>

<h2 class="text-2xl w-full dark:text-white py-8">Related components</h2>

<p class="dark:text-white text-lg w-full"><a href="https://flowbite-svelte.vercel.app/modals/small" class="text-blue-600 hover:underline dark:text-blue-500">Small Modal</a></p>

<p class="dark:text-white text-lg w-full"><a href="https://flowbite-svelte.vercel.app/modals/medium" class="text-blue-600 hover:underline dark:text-blue-500">Medium Modal</a></p>

<p class="dark:text-white text-lg w-full"><a href="https://flowbite-svelte.vercel.app/modals/large" class="text-blue-600 hover:underline dark:text-blue-500">Large Modal</a></p>

<p class="dark:text-white text-lg w-full"><a href="https://flowbite-svelte.vercel.app/modals/extra-large" class="text-blue-600 hover:underline dark:text-blue-500">Extra Large Modal</a></p>

<p class="dark:text-white text-lg w-full"><a href="https://flowbite-svelte.vercel.app/modals/signin" class="text-blue-600 hover:underline dark:text-blue-500">Signin Modal</a></p>

<p class="dark:text-white text-lg w-full"><a href="https://flowbite-svelte.vercel.app/modals/all-modals" class="text-blue-600 hover:underline dark:text-blue-500">All Modals</a></p>

<h2 class="text-2xl w-full dark:text-white py-8">References</h2>

<p class="dark:text-white text-lg"><a href="https://flowbite.com/docs/components/modal/" target="_blank" class="text-blue-600 hover:underline dark:text-blue-500">Flowbite Modal</a></p>