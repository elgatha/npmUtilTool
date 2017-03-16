# NPM Utility Tool
A tool used for Debugging!

# Installation
npm install npm_util_tool

# Code Example
```javascript
<<<<<<< HEAD
- var chalk = require('chalk');
=======
var chalk = require('chalk');
>>>>>>> origin/master

exports.debug = (title, obj, status) => {
  var seperator = '\n==================================\n';
  const output = seperator + title + seperator;

  var error = chalk.bold.red;
  console.log(error('Error!'));
  if (!status) {
    status = '';
  }
  if (process.env.DEBUG) {
    console.log(error(output), obj, status);
  }
};´´´
