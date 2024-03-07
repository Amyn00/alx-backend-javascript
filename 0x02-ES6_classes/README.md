# 0x02. ES6 classes

## Resources

**Read or watch:**

* Classes
* Metaprogramming

## Learning Objectives

* How to define a Class
* How to add methods to a class
* Why and how to add a static method to a class
* How to extend a class from another
* Metaprogramming and symbols

## Requirements

* All your files will be executed on Ubuntu 18.04 LTS using NodeJS 12.11.x
* Allowed editors: vi, vim, emacs, Visual Studio Code
* All your files should end with a new line
* A README.md file, at the root of the folder of the project, is mandatory
* Your code should use the js extension
* Your code will be tested using Jest and the command npm run test
* Your code will be verified against lint using ESLint
* Your code needs to pass all the tests and lint. You can verify the entire project running npm run full-test

## Setup

### Install NodeJS 12.11.x

(in your home directory):
```bash
curl -sL https://deb.nodesource.com/setup_12.x -o nodesource_setup.sh
sudo bash nodesource_setup.sh
sudo apt install nodejs -y
```
```bash
$ nodejs -v
v12.11.1
$ npm -v
6.11.3
```
### Install Jest, Babel, and ESLint

in your project directory, install Jest, Babel and ESList by using the supplied `package.json` and run `npm install`.

## Configuration files

Add the files below to your project directory

#### `package.json`
<details>
  <summary>Click to show/hide file contents</summary>
  ```json
  {
    "scripts": {
      "lint": "./node_modules/.bin/eslint",
      "check-lint": "lint [0-9]*.js",
      "dev": "npx babel-node",
      "test": "jest",
      "full-test": "./node_modules/.bin/eslint [0-9]*.js && jest"
    },
    "devDependencies": {
      "@babel/core": "^7.6.0",
      "@babel/preset-env": "^7.6.0",
      "@babel/node": "^7.8.0",
      "eslint": "^6.4.0",
      "eslint-config-airbnb-base": "^14.0.0",
      "eslint-plugin-import": "^2.18.2",
      "eslint-plugin-jest": "^22.17.0",
      "jest": "^24.9.0"
    }
  }
<details>
```

`**babel.config.js**`

Click to show/hide file contents

`**.eslintrc.js**`
Click to show/hide file contents

### and…

Don’t forget to run `$ npm install` when you have the `package.json`