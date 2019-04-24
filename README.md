
# Typeface Source Sans Variable

The CSS and web font files to easily self-host [Source Sans Variable](https://github.com/adobe-fonts/source-sans-pro). This package is inspired by the effort of Kyle Mathews to create [npm packages for all typefaces](https://www.bricolage.io/typefaces-easiest-way-to-self-host-fonts/) to improve loading performance.

## Install

```
npm install --save typeface-source-sans-variable
```

## Usage

This package assumes you’re using webpack to process CSS and font files. Each typeface package includes all font files for modern browsers (WOFF2 and WOFF) and a CSS file with font-face declarations pointing at these files.

You will need to have webpack or a different bundler setup to load css and font files. Many tools built with Webpack will work out of the box with Typefaces such as [Create React App](https://github.com/facebookincubator/create-react-app) and [Gatsby](https://github.com/gatsbyjs/gatsby).

Simply require the package in your project’s entry file:

```javascript
// Load the Source Sans Variable typeface
import 'typeface-source-sans-variable';
```

## Progressive enhancement

[All major browser support variable fonts as of 2018](https://caniuse.com/#feat=variable-fonts). Still, it's probably a good idea to use the following CSS selector to activate the variable font in supported browsers only:

```css
/* Checks if variable fonts are supported */
@supports (font-variation-settings: normal) {
    html {
      font-family:  "Source Sans Variable", sans-serif;
    }
}
```

