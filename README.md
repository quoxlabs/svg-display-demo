# svg-display-demo

This library allows you to

- write JSX code that specifies an SVG
- pass it to a `renderToWindow` function
- see the picture appear immediately

```ts
import { renderToWindow } from "jsr:@quoxlabs/svg-display-demo"

// Create simple SVG
const svg = 
  (<svg height="100" width="100" xmlns="http://www.w3.org/2000/svg">
    <circle r="45" cx="50" cy="50" fill="red" />
    Sorry, your browser does not support inline SVG.  
  </svg>)

// Display it
await renderToWindow(svg)
```

This is mostly a playground to have fun with Deno, Wasm, JSX, FFI, Rust, WebGPU, winding, JSR, and the integration of all of them with each other.

