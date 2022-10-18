# personal eslint config


## Installation

`yarn add -D eslint-config-kisama`

Please also make sure that you have prettier and eslint installed.

## Usage

Add "eslint-config-kisama" to "extends" array in your .eslintrc.cjs file. Make sure to put it last, so it gets the chance to override other configs.

```
require("@rushstack/eslint-patch/modern-module-resolution")

module.exports = {
  extends: [
    // ... other configs
    "eslint-config-kisama"
  ],

  // to make your prettier rules work with eslint
  rules: {
    'prettier/prettier': ['error', require('./.prettierrc.json')]
  }
}

```
