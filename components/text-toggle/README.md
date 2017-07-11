[![Published on webcomponents.org](https://img.shields.io/badge/webcomponents.org-published-blue.svg)](https://www.webcomponents.org/element/jifalops/text-toggle)

# text-toggle
Show one of two strings based on a condition. Clickability optional.

## Installation

```
bower install --save jifalops/text-toggle
```

## Usage
1. Set the true/false text values (`t` and `f`).
2. Set the `cond` property to toggle between the text values, and/or use
  the `active` property to have the text change when clicked.

## Demo
<!--
```
<custom-element-demo>
  <template is="dom-bind">
    <script src="../webcomponentsjs/webcomponents-lite.js"></script>
    <link rel="import" href="text-toggle.html">
    <style>
      text-toggle {
        font-weight: bold;
        font-family: 'monospace';
      }
      .circle {
        background-color:blue;
        height:24px;
        width:24px;
        border-radius:50%
      }
    </style>
    <next-code-block></next-code-block>
  </template>
</custom-element-demo>
```
-->

```html
<text-toggle id="ex1" t="True" f="False"></text-toggle><br/>
<button onclick="document.getElementById('ex1').toggle()">Toggle</button><p/>

<i>Click text below</i><br/>
<text-toggle active t="Clickable" f="I am"></text-toggle><p/>

<i>Circle is</i><br/>
<text-toggle active cond="{{cond}}" t="hidden" f="showing"></text-toggle>
<div hidden$="[[cond]]" class="circle"></div>

<i style="font-size:small">Polymer bindings demo may not work in this readme.</i>
```

Full demo:
[webcomponents.org](https://www.webcomponents.org/element/jifalops/text-toggle/demo/demo/index.html)
| [github](https://jifalops.github.io/text-toggle/components/text-toggle/demo/).

API: [webcomponents.org](https://www.webcomponents.org/element/jifalops/text-toggle/text-toggle)
| [github](https://jifalops.github.io/text-toggle).

## Contributing

1. Fork it on Github.
2. Create your feature branch: `git checkout -b my-new-feature`
3. Commit your changes: `git commit -am 'Add some feature'`
4. Push to the branch: `git push origin my-new-feature`
5. Submit a pull request

## License

[MIT](https://opensource.org/licenses/MIT)
