# Cata components-button

`cata-components-button` components-button styles.

Read more about how to use [SUIT CSS](https://github.com/suitcss/suit/).

## Installation

## NPM 
```
npm install cata-components-button
```

## Yarn
```
yarn add cata-components-button
```

## Download
[Download](https://github.com/raulghm/cata-components-button/releases)

## Available classes

* `Button` - [core] The core button component
* `is-disabled` - [state] For disabled-state button styles (themes)

N.B. You must also include the `disabled` attribute on `button` elements. For
`a` elements, you should prevent JavaScript event handlers from firing.

## Configurable variables

* --Button-color
* --Button-bg
* --Button-border
* --Button-border
* --Button-disabled
* --Button-padding
* --Button-border

## Use

Examples:

```html
<a class="Button" href="{{url}}">Sign up</a>

<button class="Button Button--default is-disabled" type="button">Close</button>
```

### Theming / extending

The CSS is focused on common structural requirements for buttons. You can build
your application-specific theme styles in your app. For example:

```css
@import "cata-components-button";

/**
 * Modifier: default buttons
 */

.Button--default {
  background-color: #eee;
  color: #444;
  border-color: #d9d9d9 #d9d9d9 #ccc;
  border-radius: 2px;
}

.Button--default:hover,
.Button--default:focus,
.Button--default:active,
.Button--default.is-pressed {
  background-color: #f5f5f5;
  color: #222;
  border-color: #c6c6c6 #c6c6c6 #bbb;
  box-shadow: 0 1px 2px rgba(0, 0, 0, 0.2);
}

.Button--default:focus {
  border-color: #069;
  outline: 0;
}

.Button--default:active,
.Button--default.is-pressed {
  background-color: #ccc;
  box-shadow: inset 0 1px 2px rgba(0,0,0, 0.2);
}

/**
 * Modifier: large buttons
 */

.Button--large {
  font-size: 1.5em;
  padding: 0.75em 1.5em;
}
```

## Testing

Install [Node](http://nodejs.org) (comes with npm).

```
npm install
```

To generate a build:

```
npm run build
```

To lint code with [postcss-bem-linter](https://github.com/postcss/postcss-bem-linter) and [stylelint](http://stylelint.io/)

```
npm run lint
```

To generate the testing build.

```
npm run build-test
```

To watch the files for making changes to test:

```
npm run watch
```

Basic visual tests are in `test/index.html`.

## Browser support

* Google Chrome
* Firefox
* Opera
* Safari
* Internet Explorer 9+

## Browser support

* Google Chrome
* Firefox
* Safari
* Opera
* Internet Explorer 9+
