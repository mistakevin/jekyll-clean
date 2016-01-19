This is your `_includes/` directory. This is where you can stick your "partials", like your header, footer, or anything that you want to be on multiple pages. A partial is basically a "snippet" of code that you want to reuse and keep organized. You always want to follow the DRY (Don't Repeat Yourself) principal.

For instance you probably want to put your navbar on every page. So if you typed up your navbar html:
```html
<div id="top-nav">
  <ul>
    <li>Home</li>
    <li>About Me</li>
    <li>Contact</li>
  </ul>
</div>
```
and put it into a file in here called `header.html`, you can include it whever you want!

```html
<html>
  <head>
  </head>
  <body>
    {% include header.html %}
  </body>
</html>
```

This will output
```html
<html>
  <head>
  </head>
  <body>
    <div id="top-nav">
      <ul>
        <li>Home</li>
        <li>About Me</li>
        <li>Contact</li>
      </ul>
    </div>
  </body>
</html>
```
