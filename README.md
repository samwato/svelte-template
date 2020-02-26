# Custom Svelte Template

To create a new project:

```bash
mkdir svelte-app
cd svelte-app
npx degit samwato/svelte-template .
npm i
```
## Running in development mode

Run dev mode at locahost:5000:

```bash
npm run dev
```

Install pepper-styles for global scss:

```bash
npm run styles
```

## Building and running in production mode

To create an optimised version of the app:

```bash
npm run build
```

You can run the newly built app with `npm run start`. This uses [sirv](https://github.com/lukeed/sirv), which is included in your package.json's `dependencies`


## Single-page app mode

By default, sirv will only respond to requests that match files in `public`. This is to maximise compatibility with static fileservers, allowing you to deploy your app anywhere.

If you're building a single-page app (SPA) with multiple routes, sirv needs to be able to respond to requests for *any* path. You can make it so by editing the `"start"` command in package.json:

```js
"start": "sirv public --single"
```


## Deploying to the web

### With [now](https://zeit.co/now)

Install `now` if you haven't already:

```bash
npm install -g now
```

Then, from within your project folder:

```bash
cd public
now deploy --name my-project
```


## Resources
[Svelte Docs](https://svelte.dev)
[Svelte Template](https://github.com/sveltejs/template)
[degit](https://github.com/Rich-Harris/degit)
