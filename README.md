# Moabit

Moabit is a collection of useful Sass mixins and functions.

You could actually say that Moabit is about **mixins of all beneficial, interesting things**.

## Quick start

```sh
npm install moabit --save
```

```scss
// Import default variables
// These will NOT output any CSS
@import 'moabit/variables';
@import 'moabit/functions';
@import 'moabit/mixins';

// Override default variables to match your style
// See moabit/variables.scss
@import './my-variables';

// Resets and normalizations
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
