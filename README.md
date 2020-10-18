![CoVerified Cover Image](.github/cover.jpg)

[![Netlify Status](https://api.netlify.com/api/v1/badges/3bb6d470-7937-47b9-aa89-5f7d3f53bb84/deploy-status)](https://app.netlify.com/sites/coverified-website/deploys)

# [CoVerified](https://www.coverified.info/) Website

*[CoVerified](https://www.coverified.info/) is a tool to show your websites users important and verified information about the COVID-19 outbreak*

## Contribute to fight the virus

We're using [Sapper](https://github.com/sveltejs/sapper) to build a fast and statically exported website

### Running the project

However you get the code, you can install dependencies and run the project in development mode with:

```bash
yarn
yarn dev
```

Open up [localhost:3000](http://localhost:3000) and start clicking around.

Consult [sapper.svelte.dev](https://sapper.svelte.dev) for help getting started.

### Coding guidelines

- Use CSS custom properties for variables
- Use speaking variable names (rather longer and clear than short and meaningless)
- Always use variables for colors
- Always use variables for changing (eg. media queries) or configurable values (component props / css overrides)
- Define local variables on top and global variable on `:root` or `:host`
- Use namespaced variable names:
  - Do:
    ```css
    :root {
        --color-primary: #ff00ff;
        --color-border: #ff00ff;
    }
  
    .button {
        --btn-bg-color: var(--btn-bg-color);
        --btn-border-color: var(--color-border);
        --btn-border-width: 1px;
        --btn-border-style: solid;
        
        background-color: var(--btn-bg-color-primary);
        border-color: var(--btn-border-color);
        border-width: var(--btn-border-width);
        border-style: var(--btn-border-style);
    }
    ```
  - Don't do:
    ```css
    .btn {
        --primary: #ff00ff;
        --border: 1px solid #333;
        
        background: var(--primary);
        border: var(--border);
    }
    ```

## Structure

Sapper expects to find two directories in the root of your project —  `src` and `static`.


### src

The [src](src) directory contains the entry points for your app — `client.js`, `server.js` and (optionally) a `service-worker.js` — along with a `template.html` file and a `routes` directory.


#### src/routes

This is the heart of your Sapper app. There are two kinds of routes — *pages*, and *server routes*.

**Pages** are Svelte components written in `.svelte` files. When a user first visits the application, they will be served a server-rendered version of the route in question, plus some JavaScript that 'hydrates' the page and initialises a client-side router. From that point forward, navigating to other pages is handled entirely on the client for a fast, app-like feel. (Sapper will preload and cache the code for these subsequent pages, so that navigation is instantaneous.)

**Server routes** are modules written in `.js` files, that export functions corresponding to HTTP methods. Each function receives Express `request` and `response` objects as arguments, plus a `next` function. This is useful for creating a JSON API, for example.

There are three simple rules for naming the files that define your routes:

* A file called `src/routes/about.svelte` corresponds to the `/about` route. A file called `src/routes/blog/[slug].svelte` corresponds to the `/blog/:slug` route, in which case `params.slug` is available to the route
* The file `src/routes/index.svelte` (or `src/routes/index.js`) corresponds to the root of your app. `src/routes/about/index.svelte` is treated the same as `src/routes/about.svelte`.
* Files and directories with a leading underscore do *not* create routes. This allows you to colocate helper modules and components with the routes that depend on them — for example you could have a file called `src/routes/_helpers/datetime.js` and it would *not* create a `/_helpers/datetime` route


### static

The [static](static) directory contains any static assets that should be available. These are served using [sirv](https://github.com/lukeed/sirv).

In your [service-worker.js](src/service-worker.js) file, you can import these as `files` from the generated manifest...

```js
import { files } from '@sapper/service-worker';
```

...so that you can cache them (though you can choose not to, for example if you don't want to cache very large files).


## Bundler config

Sapper uses Rollup or webpack to provide code-splitting and dynamic imports, as well as compiling your Svelte components. With webpack, it also provides hot module reloading. As long as you don't do anything daft, you can edit the configuration files to add whatever plugins you'd like.


## Production mode and deployment

To start a production version of your app, run `yarn build && yarn start`. This will disable live reloading, and activate the appropriate bundler plugins.

Run `yarn export` to create a static production build in the `__sapper__/export` dir.


## Code of Conduct

We'd like you to follow our [Code of Conduct](.github/CODE_OF_CONDUCT.md)

---

[![WirVsVirus](.github/wirvsvirus.svg)](https://wirvsvirushackathon.org/)

This project was [initially started](https://devpost.com/software/1_039_c_staatlichekommunikation_webinfowidget) during the [#wirvsvirus hackathon](https://twitter.com/hashtag/WirVsVirusHack)
