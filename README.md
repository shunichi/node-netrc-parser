# netrc-parser

[![CircleCI](https://circleci.com/gh/dickeyxxx/node-netrc-parser.svg?style=svg)](https://circleci.com/gh/dickeyxxx/node-netrc-parser)
[![codecov](https://codecov.io/gh/dickeyxxx/node-netrc-parser/branch/master/graph/badge.svg)](https://codecov.io/gh/dickeyxxx/node-netrc-parser)

# API

<!-- Generated by documentation.js. Update this documentation by updating the source code. -->

## Netrc

[src/netrc.js:188-279](https://github.com/dickeyxxx/node-netrc-parser/blob/ee085f2ba796812fab5efd40fe0b2316d20ccdd6/src/netrc.js#L188-L279 "Source code on GitHub")

parses a netrc file

### constructor

[src/netrc.js:196-205](https://github.com/dickeyxxx/node-netrc-parser/blob/ee085f2ba796812fab5efd40fe0b2316d20ccdd6/src/netrc.js#L196-L205 "Source code on GitHub")

generates or parses a netrc file

**Parameters**

-   `file` **[string](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String)** 

**Examples**

```javascript
const Netrc = require('netrc-parser')
const netrc = new Netrc()
netrc.machines['api.heroku.com'].password // get auth token from ~/.netrc
```

### save

[src/netrc.js:220-244](https://github.com/dickeyxxx/node-netrc-parser/blob/ee085f2ba796812fab5efd40fe0b2316d20ccdd6/src/netrc.js#L220-L244 "Source code on GitHub")

save the current home netrc with any changes

**Examples**

```javascript
const Netrc = require('netrc-parser')
const netrc = new Netrc()
netrc.machines['api.heroku.com'].password = 'newpassword'
netrc.save()
```
