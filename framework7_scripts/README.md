# Framework7-Scripts

This contains scripts of framework7 for version 5.1.0

## Installation

Step 1:
We recommend creating a local `.npmrc` in the project that points to GitHub Package Registry.
```
registry=https://npm.pkg.github.com/s3kdevelopers
```

Step 2:
Configure `package.json` to use the package.
```
"dependencies": {
    "@s3kdevelopers/framework7-scripts": "1.0.1"
  }
```

Step 3:
Execute command,
```
npm install
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
  'script-loader!packages/js/react/framework7-react.bundle.js',

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

### Support or Contact

Having trouble with the packages? [Contact support](mailto:support@s3kdevelopers.com) and we’ll help you sort it out.
