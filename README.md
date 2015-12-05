# gl-react-color-matrix ![](https://img.shields.io/npm/v/gl-react-color-matrix.svg) ![](https://img.shields.io/badge/gl--react->= 2.1-05F561.svg) ![](https://img.shields.io/badge/gl--react-dom%20%7C%20native-f90.svg)

[Universal](https://projectseptemberinc.gitbooks.io/gl-react/content/docs/universal.html) gl-react **color-matrix effect**

## Props

- `children` **(required)**: the content to color-matrix.
- `matrix` **(required)**: an array of 16 numbers that represents a 4x4 color matrix (rgba x rgba).

## Usage Examples

```js
var ColorMatrix = require("gl-react-color-matrix").ColorMatrix;
// or
import {ColorMatrix} from "gl-react-color-matrix";
```

## Identity

```js
<ColorMatrix matrix={[
  1, 0, 0, 0,
  0, 1, 0, 0,
  0, 0, 1, 0,
  0, 0, 0, 1
]}>
  ...
</ColorMatrix>
```

## Let only RED through

```js
<ColorMatrix matrix={[
  1, 0, 0, 0,
  0, 0, 0, 0,
  0, 0, 0, 0,
  0, 0, 0, 1
]}>
  ...
</ColorMatrix>
```

## Grayscale (approximative)

```js
<ColorMatrix matrix={[
  .3, .3, .3, 0,
  .6, .6, .6, 0,
  .1, .1, .1, 0,
   0,  0,  0, 1
]}>
  ...
</ColorMatrix>
```
