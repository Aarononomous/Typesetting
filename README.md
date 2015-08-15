# Typesetting

A Sass mixin

## About

**Typesetting** is a small set of mixins and a carefully restricted set of CSS rules for beautifying the type on your website.

### What **Typesetting** Is For

**Typesetting** makes it easy to adjust the smallest details of the lettering of your project. It&rsquo;s composed of a series of mixins which make hyphenation, Opentype set adjustment, and other advanced typography features easy to add to your project. For quickly adding professional-looking typesetting, simply link `default.css` within your HTML or include it within your CSS, or add `_default.scss` to your Sass directory.

### What **Typesetting** *Isn&rsquo;t* For

**Typesetting** is designed to complement, not supercede, your typographic stylings. It has *no* opinions on leading (line-height), font stacks, or the proportions of your headers. It does not color your links or set your margins. Adding **Typesetting** to your project will not modify any of this.

**Typesetting** is also not useful for microtypography &mdash; it cannot hang punctuation or tweak your kerning, for example &mdash; these aren&rsquo;t currently possible using only CSS.

## Usage

### CSS

To style your page with the default **Typesetting** rules, download the `typesetting.css` file and link to it in the head of your HTML document.

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

### Forking

Fork to your Sass directory. Easy!

## References

- http://typeplate.com
- http://meyerweb.com/eric/thoughts/2012/12/17/where-to-avoid-css-hyphenation
- http://www.microsoft.com/typography/otspec/featurelist.htm
- http://www.w3.org/TR/2013/CR-css-fonts-3-20131003/
- http://www.w3.org/TR/2013/WD-css-text-3-20131010/
- http://www.w3.org/TR/2002/WD-css3-linebox-20020515/
- http://blog.typekit.com/2014/02/05/kerning-on-the-web/

## License

[The MIT License](LICENSE)