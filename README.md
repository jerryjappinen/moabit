# Moabit

Moabit is a collection of useful Sass mixins and functions.

You could actually say that Moabit is about **m**ixins **o**f **a**ll **b**eneficial, **i**mportant **t**hings.

## Quick start

Install Moabit as a dependency:

```sh
npm install moabit --save
```

Import default variables, functions and mixins in your Sass files:

```scss
// Import default variables
// These will NOT output any CSS
@import '~moabit/variables';
@import '~moabit/functions';
@import '~moabit/mixins';

// Override default variables to match your style
// See moabit/variables.scss
@import './my-variables';

// Resets and normalizations (optional)
// These WILL output CSS
@import '~moabit/font-face';
@import '~moabit/normalize';

// The rest of your style codebase
// @import './defaults/forms';
// @import './foo/bar';
// @import './utilities/my-utilities';
```

## Importing in JavaScript

```js
import 'moabit/variables'
import 'moabit/functions'
import 'moabit/mixins'

import './my-custom-variables'

import 'moabit/normalize'
```

## Migration from 1.0

__Brand colors__ have been removed. Use [https://www.npmjs.com/package/brand-colors/v/2.0.0](`brand-colors`) instead.

Many __variables and mixins have been renamed__ to match natural language better. Your build pipeline will prompt you on missing mixins or variables, and you can easily look up the new version in the [source code](https://github.com/Eiskis/moabit).

`push`, `pad` and `buffer` mixins now accept a __`$step` variable__ to control the amount of margin or padding added. For example, `@include pad(2)` results in twice the normal pad.

__Device-based breakpoint mixins__ added to simplify everyday responsive development. Use `@include phone {}` to make things easy.

__Viewport mixins__ have been renamed, and the default behavior now respects the default wording. In v1, `viewport-over` would include `$breakpoint-over`, and `viewport-over-excl` had to be used to change this behavior. In v2, you can use `screen-over-or-at` and `screen-over` and get the behavior that the mixin name implies.
