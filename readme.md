# tachyons-columns 1.0.3

Tachyons CSS module of utilities for defining columns.

#### Stats

504 | 44 | 44
---|---|---
bytes | selectors | declarations

## Installation

#### With [npm](https://npmjs.com)

```
npm install --save-dev tachyons-columns
```

#### With Git

```
git clone https://github.com/tachyons-css/tachyons-columns
```

## Usage

#### Using with [PostCSS](https://github.com/postcss/postcss)

Import the css module

```css
@import "tachyons-columns";
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
<link rel="stylesheet" href="path/to/module/css/tachyons-columns">
```

#### Development

The source CSS files can be found in the `src` directory.
Running `$ npm start` will process the source CSS and place the built CSS in the `css` directory.

## The CSS

```css
/* Variables */
/* Spacing Scale - based on a ratio of 1:2 */
/* Media Queries */
/*
  COLUMNS

  A six step powers of two scale ranging from 0 to 4rem.
  Namespaces are composable and thus highly grockable - check the legend below

  Legend:

  cc = column-count
  cg = column-gap

  0 = none
  1 = 1st step in spacing scale
  2 = 2nd step in spacing scale
  3 = 3rd step in spacing scale
  4 = 4th step in spacing scale
  5 = 5th step in spacing scale

*/
.cc2 { column-count: 2; }
.cc3 { column-count: 3; }
.cc4 { column-count: 4; }
.cc5 { column-count: 5; }
.cc6 { column-count: 6; }
.cg0 { column-gap: 0; }
.cg1 { column-gap: .25rem; }
.cg2 { column-gap: .5rem; }
.cg3 { column-gap: 1rem; }
.cg4 { column-gap: 2rem; }
.cg5 { column-gap: 4rem; }
@media screen and (min-width: 48em) {
 .cc2-ns { column-count: 2; }
 .cc3-ns { column-count: 3; }
 .cc4-ns { column-count: 4; }
 .cc5-ns { column-count: 5; }
 .cc6-ns { column-count: 6; }
 .cg0-ns { column-gap: 0; }
 .cg1-ns { column-gap: .25rem; }
 .cg2-ns { column-gap: .5rem; }
 .cg3-ns { column-gap: 1rem; }
 .cg4-ns { column-gap: 2rem; }
 .cg5-ns { column-gap: 4rem; }
}
@media screen and (min-width: 48em) and (max-width: 64em) {
 .cc2-m { column-count: 2; }
 .cc3-m { column-count: 3; }
 .cc4-m { column-count: 4; }
 .cc5-m { column-count: 5; }
 .cc6-m { column-count: 6; }
 .cg0-m { column-gap: 0; }
 .cg1-m { column-gap: .25rem; }
 .cg2-m { column-gap: .5rem; }
 .cg3-m { column-gap: 1rem; }
 .cg4-m { column-gap: 2rem; }
 .cg5-m { column-gap: 4rem; }
}
@media screen and (min-width: 64em) {
 .cc2-l { column-count: 2; }
 .cc3-l { column-count: 3; }
 .cc4-l { column-count: 4; }
 .cc5-l { column-count: 5; }
 .cc6-l { column-count: 6; }
 .cg0-l { column-gap: 0; }
 .cg1-l { column-gap: .25rem; }
 .cg2-l { column-gap: .5rem; }
 .cg3-l { column-gap: 1rem; }
 .cg4-l { column-gap: 2rem; }
 .cg5-l { column-gap: 4rem; }
}
```

## Contributing

1. Fork it
2. Create your feature branch (`git checkout -b my-new-feature`)
3. Commit your changes (`git commit -am 'Add some feature'`)
4. Push to the branch (`git push origin my-new-feature`)
5. Create new Pull Request

## Authors

- [Alec Lomas](http://lowmess.com)

## License

MIT

