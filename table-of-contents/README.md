# Table Of Contents Shortcode

## Install Module

Add the following code to your module list in the `config/_default/module.toml` file.

```toml
[[imports]]
path = "github.com/flowqi-dev/web-modules/table-of-contents"
```

Add the following code to your `assets/scss/main.scss` or `assets/scss/style.scss` file.

```scss
@import 'toc';
```

<hr>

## Customize Table Of Contents

```toml
[markup.tableOfContents]
startLevel = 2
endLevel = 5
ordered = true
```

<hr>

## Use it as a Shortcode

```md
{{< toc >}}
```

<hr>

## Use it as a Partial

available parameters:

* Class = "your-class"
* Collapsed: display as collapsed | default true

```html
{{ partial "toc.html" }}
```
