# NPM Utility Tool
A tool used for Debugging!

# Installation
npm install npm_util_tool

# Usage
In order to start the debug tool you must add "DEBUG=true" in the front of "nodemon lib/util.js"

## Example Usage

```
const util = require('./util');

//bump versions (patch, minor, major)
const patch = util.bump('3.3.3', 'patch');
const minor = util.bump('3.3.3', 'minor');
const major = util.bump('3.3.3', 'major');

//success
util.debug('patch', patch, false);
util.debug('minor', minor, true);

//error
util.debug('major', major, false);

```
