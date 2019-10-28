# Framework7-Scripts

This contains scripts of framework7 for version 5.1.0

## Installation

```
npm install @s3kdevelopers/framework7-scripts@1.0.1
```

Or add this package to your `package.json` file:

```
"dependencies": {
    "@s3kdevelopers/framework7-scripts": "1.0.1"
  }
```

## Usage

```
const myPackage = require('@s3kdevelopers/framework7-scripts');
myPackage.helloWorld();
```

## For React JS

Load the scripts in webpack
```
entry: [
  'script-loader!packages/js/core/framework7.bundle.min.js',

],
alias: {
  applicationStyles: 'app/styles/app.scss'
},,
```

import the CSS file in app.scss
```
@import 'packages/css/framework7.bundle';
```

Load the files in app.jsx
```
require('style-loader!css-loader!sass-loader!applicationStyles');
```
