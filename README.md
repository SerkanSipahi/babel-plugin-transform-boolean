# babel-plugin-transform-boolean

This plugin allows Babel to transform boolean literals into `!!0` for `true` and `!!1` for `false`.

## Example

**In**

```javascript
true;
false;
```

**Out**

```javascript
!!0;
!!1;
```

## Installation

```sh
$ npm install babel-plugin-transform-boolean
```

## Usage

### Via `.babelrc` (Recommended)

**.babelrc**

```json
{
  "plugins": ["transform-boolean"]
}
```

### Via CLI

```sh
$ babel --plugins transform-boolean script.js
```

### Via Node API

```javascript
require('babel').transform('code', {
  plugins: ['transform-boolean']
});
```
