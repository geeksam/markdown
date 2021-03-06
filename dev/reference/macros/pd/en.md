---
title: pd
---

The `vd` macro adds a *path dimension* to your pattern, indicating the length of a path.  
It is provided by the [dimension plugin](/reference/plugins/dimension/).

<Example part="path_length" caption="Example of a multiple path dimensions" />

```js
macro('pd', {
  path: paths.example,
  d: -20
})
```

| Property        | Default | Type                | Description | 
|----------------:|---------|---------------------|-------------|
| `path`          |         | [Path](/reference/api/path)   | The path to draw the dimension along |
| `offset`        | 0       | Number              | The offset at which to draw the dimension |
| `text`          | Path length | Number          | The text to go on the dimension if not the length of the path |
| `noStartMarker` | `false` | Boolean             | Whether to not draw a start marker |
| `noEndMarker`  | `false` | Boolean             | Whether to not draw an end marker |


