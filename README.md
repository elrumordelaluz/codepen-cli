# codepen-cli

The live editor of [CodePen](https://codepen.io/) is not stable for me most of the time due to the network (in China...), so I always write demos on my local machine first,
then open CodePen afterwards and copy/paste into the editor.

This tool is for saving this process by doing the following steps:

1. Extract *external* or *inline* **scripts** and **styles** of a local HTML file.
2. Open a new CodePen editor with default browser.
3. Prefill each html/js/css section and external depencencies in the editor automatically.

The rest is to click the **SAVE** button.

## Installation

```bash
$ npm install -g @yuanchuan/codepen-cli
```

## Example

```bash
$ codepen index.html
```

It can be used to preview a `markdown` file quickly on CodePen:

```bash
$ codepen README.md
```

Edit a JS file on CodePen:

```bash
$ codepen example.js
```

## Options

#### keep-inline

By default all the **inline** script/style in HTML will be put into js/css sections seperatly,
but they can stay with the HTML using `keep-inline` option.

```bash
$ codepen index.html --keep-inline
```


## References

[https://blog.codepen.io/documentation/prefill](https://blog.codepen.io/documentation/prefill/)


## Usage

```
Usage:
  codepen <filename>

Options:
  --keep-inline: Keep inline styles/scripts inside html
  --help:        Display help info

Supported filename types by extension:
  htm, html, md, markdown, js, ts, css, less, sass, scss, styl
```
