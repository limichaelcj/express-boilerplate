Express Boilerplate
===================
###### For Linux systems

### Usage
In the root directory, generate a new express.js template with:
```bash
bash generate <options>
```
### Options
- `-env`: Include `dotenv` package and create `.env` file in root
- `-pug`: Include `pug` package and set express view engine to pug
- `-db`: Include `mongoose` package for accessing MongoDB database via MVC framework <sub>_(**includes** -env)_</sub>
- `-bcrypt`: Include `bcrypt` package for password encryption
- `-helmet`: Include `helmet` package for secure HTTP headers
- `-session`: Include `express-session` package to implement session cookies <sub>_(**includes** -env)_</sub>
- `-passport`: Include `passport` packages for user authentication <sub>_(**includes** -env, -session)_</sub>
- `-socket`: Include `socket.io` packages for real-time server-client communication <sub>_(**includes** -env, -session, -passport)_</sub>
- `-r`, `-remove`: Auto-remove the generate script after running it.
### Notes
- Files will be generated in the current working directory and the generate script can be deleted afterward.
- Node.js must be installed on your computer to run the script properly.
- Remember to change the `package.json` and `.env` files according to your app after running the generate script.

### Example

```bash
# ../express-boilerplate
bash generate -pug -db -bcrypt -passport
# Generates a template with dotenv, pug, mongoose, bcrypt, express-session, and passport preconfigured
```
