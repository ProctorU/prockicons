# ProctorU prockicons, forked from GitHub's octicons.

## Install

**NOTE:** The compiled files are located in `build/`. This directory is located in the published npm package. Which means you can access it when you `yarn add prockicons`. You can also build this directory by following the [building prockicons directions](#building-prockicons). The files in the `lib/` directory are the raw source files and are not compiled or optimized.

#### Usage

```bash
$ yarn add prockicons
```

```js
import prockicons from 'prockicons'

prockicons.camera
```

#### `prockicons.camera.toSVG()`

Returns a string of the `<svg>` tag.

```js
prockicons.camera.toSVG()
// <svg version="1.1" width="12" height="16" viewBox="0 0 12 16" class="prockicons prockicons-camera" aria-hidden="true"><path d="M7.48 8l3.75 3.75-1.48 1.48L6 9.48l-3.75 3.75-1.48-1.48L4.52 8 .77 4.25l1.48-1.48L6 6.52l3.75-3.75 1.48 1.48z"/></svg>
```

The `.toSVG()` method accepts an optional `options` object. This is used to add CSS classnames, a11y options, and sizing.

##### class

Add more CSS classes to the `<svg>` tag.

```js
prockicons.camera.toSVG({ "class": "close" })
// <svg version="1.1" width="12" height="16" viewBox="0 0 12 16" class="prockicons prockicons-camera close" aria-hidden="true"><path d="M7.48 8l3.75 3.75-1.48 1.48L6 9.48l-3.75 3.75-1.48-1.48L4.52 8 .77 4.25l1.48-1.48L6 6.52l3.75-3.75 1.48 1.48z"/></svg>
```

## Building Prockicons

All the files you need will be in the `build/` directory already, but if you’ve made changes to the `lib/` directory and need to regenerate, follow these steps:

1. Open the Prockicons directory in Terminal
2. `yarn install` to install all dependencies for the project.
3. Run the command `yarn run build`. This will run the grunt task to build the SVGs, placing them in the `build/` directory.


## License

> Forked from GitHub's Octicons. Thank you :)

(c) 2012-2016 GitHub, Inc.

When using the GitHub logos, be sure to follow the [GitHub logo guidelines](https://github.com/logos).

_SVG License:_ [SIL OFL 1.1](http://scripts.sil.org/OFL)  
Applies to all SVG files

_Code License:_ [MIT](./LICENSE)  
Applies to all other files
