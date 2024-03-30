# Palm Tree Core Module

This is the core module for the Palm Tree Design System. It contains the base styles that will be used in all the other modules.

## Scripts

This project runs on `node.js`. Install [Node](https://nodejs.org/) for npm to use.

Run `npm install` in the project directory and make sure it passes.

In this project you can run the following Scripts:

### `npm css-compile`

Compile all the sass code into the `./src/scss/` folder. \
Use `_` at the beginning of any `.scss` file so it won't compile.

### `npm run css-minify`

Does the same as `npm css-compile` and then minifies the compiled files. \
This is very useful when uploading a file to production.

## Folder Structure

### Main file

The main file (usually labelled `main.scss`) should be the only Sass file from the whole code base not to begin with an underscore. This file should not contain anything but `@import` and comments.

_Note: when using [Eyeglass](https://github.com/sass-eyeglass/eyeglass) for distribution, it might be a fine idea to name this file `index.scss` rather than `main.scss` in order to stick to [Eyeglass modules specifications](https://github.com/sass-eyeglass/eyeglass#writing-an-eyeglass-module-with-sass-files). See [#21](https://github.com/KittyGiraudel/sass-boilerplate/issues/21) for reference._

Reference: [Sass Guidelines](http://sass-guidelin.es/) > [Architecture](http://sass-guidelin.es/#architecture) > [Main file](http://sass-guidelin.es/#main-file)

### Elements

The `elements/` is one of the main features of the architecture. It contains styles for base elements, such as links, paragraphs, headings, etc. It is a way to apply base styles to elements without using classes. Just needs to use semantic and accessible HTML.
