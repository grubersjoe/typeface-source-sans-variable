
# Typeface Source Sans Variable

The CSS and web font files to easily self-host **Source Sans Variable**. This package is inspired by the effort of Kyle Mathews to create [NPM packages for all typefaces](https://www.bricolage.io/typefaces-easiest-way-to-self-host-fonts/).

## Install

`npm install --save typeface-source-sans-variable`

## Usage

Typefaces assume you’re using webpack to process CSS and files. Each typeface
package includes all font files for modern browsers (WOFF2 and WOFF) and
a CSS file with font-face declarations pointing at these files.

You will need to have webpack setup to load css and font files. Many tools built
with Webpack will work out of the box with Typefaces such as [Gatsby](https://github.com/gatsbyjs/gatsby)
and [Create React App](https://github.com/facebookincubator/create-react-app).

To use, simply require the package in your project’s entry file e.g.

```javascript
// Load Source Sans Variable typeface
require('typeface-source-sans-variable')
```
