# Deno SvelteKit Template

This template application uses
[SvelteKit](https://kit.svelte.dev/docs/introduction) and provides a starting
point for using SvelteKit on [Deno Deploy](https://deno.com/deploy).

## Local development

Begin by installing the dependencies for the project:

```bash
npm install
```

Start the development server on `http://localhost:3000`:

```bash
npm run dev
```

## Run on Deno Deploy

This repo contains a GitHub workflow configuration to automatically deploy your
application when you push to the main branch.

Before deploying for the first time, edit `.github/workflows/deploy.yml` and
include your project ID near the bottom of this file.

### Previewing production build

To preview the production version of the application, build the site with this
command:

```bash
npm run build
```

Then, run the server:

```bash
cd build
deno run -A --unstable index.js
```

Check out the [SvelteKit](https://kit.svelte.dev/docs/introduction) docs for
more information.

## License

MIT
