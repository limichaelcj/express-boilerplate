Express Boilerplate
===================

### Usage
Generate a new express.js template with:
```bash
bash generate <options>
```

### Options
`-env`: Include `dotenv` package and create `.env` file in root.
`-pug`: Include `pug` package and set express view engine to pug.
`-db`: Include `mongoose` package for accessing MongoDB database via MVC framework. _(Includes env)_
`-bcrypt`: Include `bcrypt` package for password encryption.
`-helmet`: Include `helmet` package for securing HTTP headers
`-session`: Include `express-session` package to implement session cookies. _(Includes env)_
`-passport`: Include `passport` package for user authentication. _(Includes env, session)_
`-socket`: Include `socket.io` package for real-time server-client communication. _(Includes env, session, passport)_

### Example

```bash
bash install -pug -db -bcrypt -passport
# Generates a basic express boilerplate with pug.js mongoose.js bcrypt.js and passport.js preconfigurations
```
