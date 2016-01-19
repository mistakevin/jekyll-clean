This is your `_layouts/` directory. This is where you put your "wrappers" that you would like to "extend". Let's look at an example.

In a layout called `_layouts/default.html`, you could have something like:
```html
<html>
  <head>
  </head>
  <body>
    {{  content }}
  </body>
</html>
```

Then when you create a page, like `index.html`, you could put:

```html
---
layout: default
---

<h1> Hello World!</h1>
```

Then when you view your generated site, you'd see:

```html
<html>
  <head>
  </head>
  <body>
    <h1> Hello World!</h1>
  </body>
</html>
```

The `{{ content }}` in your layout is where the content of the template that is extending the layout goes! (that's a mouthful)