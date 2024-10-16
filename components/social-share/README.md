# Social share components

## Install Module

Add the following code to your module list in the `config/_default/module.toml` file.

```toml
[[imports]]
path = "github.com/flowqi-dev/web-modules/components/social-share"
```

Add the following code to your `assets/scss/main.scss` or `assets/scss/style.scss` file.

```scss
@import 'social-share';
```

<hr>

## Share Implementation

Call it, as a partial in your theme.

Available parameters:

* `Context`: .
* `Class`: wrapper class
* `Title`: share title
* `Facebook`: share facebook | default true
* `Twitter`: share twitter | default true
* `Email`: share email | default true
* `Reddit`: share reddit | default true
* `Whatsapp`: share whatsapp | default true
* `Telegram`: share telegram | default true
* `Linkedin`: share linkedin | default true
* `Pinterest`: share pinterest | default true
* `Tumblr`: share tumblr | default true
* `Vk`: share vk | default true

  
```html
<!-- social share -->
{{ partial "social-share.html" (dict "Context" .) }}
```
