# tachyons-columns 1.0.2

Tachyons CSS module of utilities for defining columns.

#### Stats

601 | 44 | 132
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
.cc2 { -webkit-column-count: 2; -moz-column-count: 2; column-count: 2; }
.cc3 { -webkit-column-count: 3; -moz-column-count: 3; column-count: 3; }
.cc4 { -webkit-column-count: 4; -moz-column-count: 4; column-count: 4; }
.cc5 { -webkit-column-count: 5; -moz-column-count: 5; column-count: 5; }
.cc6 { -webkit-column-count: 6; -moz-column-count: 6; column-count: 6; }
.cg0 { -webkit-column-gap: 0; -moz-column-gap: 0; column-gap: 0; }
.cg1 { -webkit-column-gap: .25rem; -moz-column-gap: .25rem; column-gap: .25rem; }
.cg2 { -webkit-column-gap: .5rem; -moz-column-gap: .5rem; column-gap: .5rem; }
.cg3 { -webkit-column-gap: 1rem; -moz-column-gap: 1rem; column-gap: 1rem; }
.cg4 { -webkit-column-gap: 2rem; -moz-column-gap: 2rem; column-gap: 2rem; }
.cg5 { -webkit-column-gap: 4rem; -moz-column-gap: 4rem; column-gap: 4rem; }
@media screen and (min-width: 48em) {
 .cc2-ns { -webkit-column-count: 2; -moz-column-count: 2; column-count: 2; }
 .cc3-ns { -webkit-column-count: 3; -moz-column-count: 3; column-count: 3; }
 .cc4-ns { -webkit-column-count: 4; -moz-column-count: 4; column-count: 4; }
 .cc5-ns { -webkit-column-count: 5; -moz-column-count: 5; column-count: 5; }
 .cc6-ns { -webkit-column-count: 6; -moz-column-count: 6; column-count: 6; }
 .cg0-ns { -webkit-column-gap: 0; -moz-column-gap: 0; column-gap: 0; }
 .cg1-ns { -webkit-column-gap: .25rem; -moz-column-gap: .25rem; column-gap: .25rem; }
 .cg2-ns { -webkit-column-gap: .5rem; -moz-column-gap: .5rem; column-gap: .5rem; }
 .cg3-ns { -webkit-column-gap: 1rem; -moz-column-gap: 1rem; column-gap: 1rem; }
 .cg4-ns { -webkit-column-gap: 2rem; -moz-column-gap: 2rem; column-gap: 2rem; }
 .cg5-ns { -webkit-column-gap: 4rem; -moz-column-gap: 4rem; column-gap: 4rem; }
}
@media screen and (min-width: 48em) and (max-width: 64em) {
 .cc2-m { -webkit-column-count: 2; -moz-column-count: 2; column-count: 2; }
 .cc3-m { -webkit-column-count: 3; -moz-column-count: 3; column-count: 3; }
 .cc4-m { -webkit-column-count: 4; -moz-column-count: 4; column-count: 4; }
 .cc5-m { -webkit-column-count: 5; -moz-column-count: 5; column-count: 5; }
 .cc6-m { -webkit-column-count: 6; -moz-column-count: 6; column-count: 6; }
 .cg0-m { -webkit-column-gap: 0; -moz-column-gap: 0; column-gap: 0; }
 .cg1-m { -webkit-column-gap: .25rem; -moz-column-gap: .25rem; column-gap: .25rem; }
 .cg2-m { -webkit-column-gap: .5rem; -moz-column-gap: .5rem; column-gap: .5rem; }
 .cg3-m { -webkit-column-gap: 1rem; -moz-column-gap: 1rem; column-gap: 1rem; }
 .cg4-m { -webkit-column-gap: 2rem; -moz-column-gap: 2rem; column-gap: 2rem; }
 .cg5-m { -webkit-column-gap: 4rem; -moz-column-gap: 4rem; column-gap: 4rem; }
}
@media screen and (min-width: 64em) {
 .cc2-l { -webkit-column-count: 2; -moz-column-count: 2; column-count: 2; }
 .cc3-l { -webkit-column-count: 3; -moz-column-count: 3; column-count: 3; }
 .cc4-l { -webkit-column-count: 4; -moz-column-count: 4; column-count: 4; }
 .cc5-l { -webkit-column-count: 5; -moz-column-count: 5; column-count: 5; }
 .cc6-l { -webkit-column-count: 6; -moz-column-count: 6; column-count: 6; }
 .cg0-l { -webkit-column-gap: 0; -moz-column-gap: 0; column-gap: 0; }
 .cg1-l { -webkit-column-gap: .25rem; -moz-column-gap: .25rem; column-gap: .25rem; }
 .cg2-l { -webkit-column-gap: .5rem; -moz-column-gap: .5rem; column-gap: .5rem; }
 .cg3-l { -webkit-column-gap: 1rem; -moz-column-gap: 1rem; column-gap: 1rem; }
 .cg4-l { -webkit-column-gap: 2rem; -moz-column-gap: 2rem; column-gap: 2rem; }
 .cg5-l { -webkit-column-gap: 4rem; -moz-column-gap: 4rem; column-gap: 4rem; }
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

