# PrettyJSON
A lightweight JavaScript library for pretty and customisable JSON formatting of strings or objects.

## Basic Usage
- Just include `pretty-json.js`, and then call `prettify(j)` on your JSON object or string `j`.
- Formatting works best if you wrap the output in a `<pre>`.

## Advanced Usage
You can customise the tab size and colors returned by `prettify()`, for example:

```js
var newColors = {
    'boolean': '#6e45ab',
    'null': 'magenta',
    'key': 'green'
}
document.write('<pre>'+prettify(j, 4, newColors)+'</pre>');
```

will set the tab size to `4` and override the default colors for booleans, nulls, and keys:

![Alt text](/example_output.png)