# Simple Readme Style

Simple HTML ReadMe-like style for use in other projects.

## About

This package provides a very basic CSS for ReadMe-like HTML projects that need a simple styling.

## Features

### Automatic highlighting for standard HTML tags

Standard HTML tags are automatically highlighted.

Currently supported tags:

- `<h1>`, `<h2>`: Are displayed with a bottom border, like in GitHub's Markdown Viewer.
- `<a>`: Are displayed in a blue that fits the background color.
- `<header>`: With a text alignment to the right.

### Dark and light mode

The styling supports both light and dark mode.
The theme is determined from the system preferences.

### Centered content

The page content inside `<div class="page-content"> ... </div>"` is displayed centered with a maximum width.

## Installation

This package is provided in GitHub's NPM Registry. To get started, create a file `.npmrc` and add the following content:

```
@doba16:registry=https://npm.pkg.github.com
```

Other methods to use a package from GitHub's NPM Registry can be found at [GitHub's Documentation](https://docs.github.com/en/packages/working-with-a-github-packages-registry/working-with-the-npm-registry).

After that, install the npm package using yarn or npm.

```bash
# Using NPM
npm install @doba16/simple-readme-style

# Using Yarn
yarn add @doba16/simple-readme-style@1.0.0
```

## Usage

The CSS can be included in different ways. Both are tested with [parcel](https://parceljs.org/).

### Using html link tag

The CSS can be included using a simple HTML link tag.

```html
<!DOCTYPE html>
<html lang="en">
<head>
    <link rel="stylesheet" href="../node_modules/@doba16/simple-readme-style/css/simple-readme-style.css">
</head>
<body>
    <div class="page-content">
        <h1>Content</h1>
        Content goes here...
    </div>
</body>
</html>
```

### Import in JavaScript

Import CSS in JavaScript or TypeScript.

```js
import "@doba16/simple-readme-style/css/simple-readme-style.css"
```
