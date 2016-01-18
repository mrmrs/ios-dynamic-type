# ios-dynamic-type 1.0.0

CSS module for utilizing dynamic type in iOS on the web

#### Stats

591 | 14 | 13
---|---|---
bytes | selectors | declarations

## Installation

#### With [npm](https://npmjs.com)

```
npm install --save-dev ios-dynamic-type
```

#### With Git

```
git clone https://github.com/tachyons-css/ios-dynamic-type
```

## Usage

#### Using with [PostCSS](https://github.com/postcss/postcss)

Import the css module

```css
@import "ios-dynamic-type";
```

Then process the CSS using the [`tachyons-cli`](https://github.com/tachyons-css/tachyons-cli)

```sh
$ npm i -g tachyons-cli
$ tachyons-cli path/to/css-file.css > dist/t.css
```

#### Using the CSS

The built CSS is located in the `css` directory. It contains an unminified and minified version.
You can either cut and paste that css or link to it directly in your html.

```html
<link rel="stylesheet" href="path/to/module/css/ios-dynamic-type">
```

#### Development

The source CSS files can be found in the `src` directory.
Running `$ npm start` will process the source CSS and place the built CSS in the `css` directory.

## The CSS

```css
/*

  iOS SYSTEM FONTS

  For utilitizing the adaptive type behavior that is available on iOS devices.

*/
html, body { font-family: -apple-system; }
/*

  https://webkit.org/blog/3709/using-the-system-font-in-web-content/

  "Going beyond the system font, iOS has dynamic type behavior, which can provide
  an additional level of fit and finish to your content. These text styles
  identify more than simply a particular font family; instead, they represent an
  entire style, including size and weight. These styles are therefore
  characterized by values given to the more-general font CSS property."

  Below are single purpose classes for using adaptive type on the web. This will only
  work for iOS devices so you'll likely want some fall-backs.

*/
.ios-body { font: -apple-system-body; }
.ios-headline { font: -apple-system-headline; }
.ios-subheadline { font: -apple-system-subheadline; }
.ios-caption { font: -apple-system-caption1; }
.ios-caption2 { font: -apple-system-caption2; }
.ios-footnote { font: -apple-system-footnote; }
.ios-short-body { font: -apple-system-short-body; }
.ios-short-headline { font: -apple-system-short-headline; }
.ios-short-subheadline { font: -apple-system-short-subheadline; }
.ios-short-caption { font: -apple-system-short-caption1; }
.ios-short-footnote { font: -apple-system-short-footnote; }
.ios-tall-body { font: -apple-system-tall-body; }
```

## Contributing

1. Fork it
2. Create your feature branch (`git checkout -b my-new-feature`)
3. Commit your changes (`git commit -am 'Add some feature'`)
4. Push to the branch (`git push origin my-new-feature`)
5. Create new Pull Request

## Authors

* [mrmrs](http://mrmrs.io)
* [johno](http://johnotander.com)

## License

MIT

