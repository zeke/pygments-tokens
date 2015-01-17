# pygments-tokens

A map of the tokens used by the pygments syntax highlighter

[Pygments](http://pygments.org/) is a syntax highlighter that
supports over 300 programming languages.  To use pygments in node,
check out [pygmentize-bundled](https://github.com/rvagg/node-pygmentize-bundled) or
[other options on npm](https://www.npmjs.com/search?q=pygments).

Given this JavaScript string:

```js
var a = "b";
```

pygments will generate this HTML:


```html
<div class="highlight"><pre>
  <span class="kd">var</span>
  <span class="nx">a</span>
  <span class="o">=</span>
  <span class="s2">&quot;b&quot;</span>
  <span class="p">;</span>
</pre></div>
```

See the `kd`, `nx`, `o` classes above? This package exports a map of [all the tokens used by pygments](http://pygments.org/docs/tokens/).

Use it to generate and/or validate pygments CSS stylesheets, or to create
a whitelist of allowable CSS class names.
