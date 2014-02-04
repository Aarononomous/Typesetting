# Typesetting, a Sass Mixin

## About

Typesetting is a small set of mixins and a carefully restricted set of CSS rules for beautifying the type on your website.

### What This Is For

Typesetting makes it easy to adjust the smallest details of the lettering of your project. It's composed of a series of mixins which make hyphenation, Opentype set adjustment, and other advanced typography features easy to add to your project. For quickly adding professional-looking typesetting, simply include `default.css` or `_default.scss`.

### What This Is Not For

Typesetting is designed to complement, not supercede, your typographic stylings. It has *no* opinions on leading (line-height), font stacks, or the proportions of your headers. It does not color your links or set your margins. Adding Typesetting to your project will not modify any of this.

Typesetting is also not useful for microtypography--it cannot hang punctuation--this isn't currently possible with CSS.

## Usage

### CSS

To style your page with the default Typesetting rules, download the `typesetting.css` file and link to it in the head of your HTML document. 

```HTML
<head>
  ...
  <link rel="stylesheet" href="/path/to/a/framework/that/needs/to/come/first.css" />
  <link rel="stylesheet" href="/typesetting/default.css" />
  <link rel="stylesheet" href="/path/to/your/sylesheet.css" />
  ...
</head>
```

Alternatively, import it into your base CSS file.

```CSS
@import("path/to/typesetting/default.css");
```


### SCSS

There are a few ways to use this in your project.

1. Import the default SCSS file:

	```SCSS
	@import "typesetting/default"; // At the top of your SCSS file
	```

2. Import the specific mixins you need:

	```SCSS
	@import "typesetting/hyphenate", "typesetting/font-feature-settings";
	```
3. Import *all* of the mixins *without* the default styling:
	```SCSS
	@import "typesetting";
	```

## License

The MIT License