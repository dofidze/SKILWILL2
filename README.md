დავალება 
Js

const validator = require("validator");

console.log(validator.isEmail(`test@test.com`)); //true
console.log(validator.isEmail(`abcDE123`)); //false

package.json

{
  "name": "my-first-project",
  "version": "1.0.0",
  "description": "",
  "main": "main.js",
  "scripts": {
    "test": "echo \"Error: no test specified\" && exit 1"
  },
  "author": "misho",
  "license": "ISC",
  "dependencies": {
    "is-number": "^7.0.0",
    "validator": "^13.9.0"
  }
}
