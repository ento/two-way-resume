Two-Way Résumé Template
---------

Résumé (CV) website template for creating [a two-way résumé](https://observablehq.com/ento/the-two-way-resume). Based on [universal-resume](https://github.com/WebPraktikos/universal-resume).


How to run it
---------

Navigate to the base directory:

```
cd two-way-resume
```

Install dependencies:

```
npm install
```

Start the development server:

```
npm run serve
```

Only build HTML and generate CSS that is used on the page which results in a much smaller file size:

```
npm run build
```

Differences from universal-resume
---------

`index.html` is the main content file, not `docs/index.html`.

For a bit of privacy via obscurity, the build step uses [`envsub`](https://www.npmjs.com/package/envsub) to substitue `${ENVVARS}` with the values of the corresponding environment variables.

One way to set up environment variables to be used during the build process is through Netlify: `netlify.toml` includes minimum config for connecting the repo to a Netlify site. Environment variables can be configured in the site settings and running `netlify build` locally will feed them to `envsub`.


License
---------

NonCommercial-ShareAlike 1.0 Generic (CC NC-SA 1.0)
https://creativecommons.org/licenses/nc-sa/1.0/

### You are free to:

Share — copy and redistribute the material in any medium or format

Adapt — remix, transform, and build upon the material

### Under the following terms:

NonCommercial — You may not use the material for commercial purposes.

ShareAlike — If you remix, transform, or build upon the material, you must distribute your contributions under the same license as the original.
