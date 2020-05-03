# Svelte UI Components Boilerplate with Tailwindcss and Pug

**You can create your own component library with this boilerplate.**

A base for building Svelte components library using tailwindcss and pug.

## Using

**On GitHub:**

`Use this template` button on top right.

**CLI:**

1. Clone it with [degit](https://github.com/Rich-Harris/degit)

```bash
npx degit fredpies/ui-library-boilerplate your-directory
cd ui-library-boilerplate
npm install # or yarn
```

2. Add your component's code to [src/](./src/) as directory, e.g.: [src/TestComponent/](src/Test/) (or add your component directly to [src/](./src/)).

3. Export the new component to apps in [src/index.js](./src/index.js)

4. [src/test.js](./src/test.js) and [src/App.svelte](./src/App.svelte) are for testing purposes:

-   add component to the [src/App.svelte](./src/App.svelte)
-   add component's properties to [src/test.js](./src/test.js)

4. Create your test cases to your component:

-   add tests to [test/](./test/) directory

## Development

1. `npm install`

2. `npm run dev` :

-   **build components on change** and
-   **serves** from `public/` directory at `http://localhost:5000`
-   and **handling livereload**

3. `npm test` : test runner

For changing the view of the test page use [tailwind-entry.css](./tailwind-entry.css) and [public/index.html](./public/index.html)

## Using components in app

https://github.com/rollup/rollup-plugin-svelte#pkgsvelte

**Tip:** You can use _component library,_ and install it _once_ as **devDependencies** to app with `npm i -D <path-to-your-components>`.

Import _component library_ into your app in `App.svelte` :

```html
<script>
    import { Test } from 'ui-library-boilerplate'
</script>

<Test />
```

## Technical background

-   `svelte` https://svelte.dev
-   `nightwatch` for testing: https://nightwatchjs.org
-   `eslint` and `prettier` for formatting and linting
-   `rollupjs` for bundling: https://rollupjs.org
