# Moabit

Moabit is a collection of useful Sass mixins and functions.

You could actually say that Moabit is about **mixins of all beneficial, interesting things**.

## Quick start

```sh
npm install moabit --save
```

```scss
// Import default variables
@import 'moabit';

// Override default variables
// See moabit/variables.scss
@import './variables';

// Resets and normalizations
@import 'moabit/normalize';

// The rest of your style codebase
@import '.global.scss';
```

## What's included

```js
import 'moabit/variables'
import 'moabit/functions'
import 'moabit/mixins'
import 'moabit/normalize'

import './my-custom-variables'
```

Or your Sass files:

```scss
@import 'moabit/variables';
@import 'moabit/functions';
@import 'moabit/mixins';
@import 'moabit/normalize';

@import './my-custom-variables';
```
