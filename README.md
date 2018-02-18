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
@import 'moabit/variables';
@import 'moabit/functions';
@import 'moabit/mixins';

// Override default variables to match your style
// See moabit/variables.scss
@import './my-variables';

// Resets and normalizations (optional)
// These WILL output CSS
@import 'moabit/font-face';
@import 'moabit/normalize';

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
