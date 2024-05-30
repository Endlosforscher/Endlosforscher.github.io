+++
title = 'Introduction to Suex'
date = 2024-05-30T14:07:16+02:00
draft = false
+++

# Introduction {#introduction}

Disclaimer: Suex is not a real frontend framework; it's just an example of documentation written using [Hugo](https://gohugo.io).

### What is Suex?

**Suex** is essentially a **simple project** designed by @Endlosforscher to test the capabilities of **Hugo** and the power of **Server-Side Rendering (SSR)**. It serves as a sort of **documentation** for a **JavaScript frontend framework** that enables the **rapid creation of robust interfaces**.


### Basic Example

```js
import { createApp, reference } from 'suex'

createApp({
  setup() {
    const count = reference(0);
    return { count };
  }
}).insertIn('#myDiv')
```

```html
/* Markup */
<div id="myDiv">
  <button _click="count++">
      My count is : {{count}}
  </button>
</div>
```