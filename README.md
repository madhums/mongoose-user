## mongoose-user
Some generic methods, statics and virtuals used for user schemas

## Installation

```sh
$ npm install mongoose-user
```

or include it in `package.json`

## Usage

```js
var mongoose = require('mongoose')
var userPlugin = require('mongoose-user')

var UserSchema = new mongoose.Schema({
  name: { type: String, default: '' },
  email: { type: String, default: '' },
  username: { type: String, default: '' },
  hashed_password: { type: String, default: '' },
  salt: { type: String, default: '' }
})

UserSchema.plugin(userPlugin, {})

mongoose.model('User', UserSchema)
```

## License
MIT
