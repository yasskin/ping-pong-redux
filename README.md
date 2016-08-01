# _JavaScript Workflow [ gulp | node | browserify ]_

#### _Epicodus: JavaScript (Week 1), August 1, 2016_

#### By _**Marty Fitchen**_ + _**Noah Yasskin**_

## Description

_This is an Epicodus student lesson creating the workflow checklist for JavaScript. See specs below:_

_Ping Pong_
 a function which would display the numbers from 1 to a goal number chosen by the user, replacing those divisible by 3 with the word "ping", those divisible by 5 with the word "pong" and those divisible by both with "ping-pong".

_Calculator_
_A basic calculator app. The calculator object includes the pingPong method. It has:_

 * _npm packages_
 * _a gulpfile_
 * _file structure_

 _It also has standard arithmetic methods such as +, -, *, /.
 These methods are called on a single Calculator object in a front-end file whenever the user submits the appropriate form. Then, it displays the results:_

 * _The front-end interface file gets user input and displays results_
 * _The calculations should be done on the back-end as part of the Calculator object._

Steps:
1. Start with some basic HTML and jQuery to create functions to take care of whatever logic the problem calls for.
2. Then, we refactor by using objects and splitting our JavaScript into multiple files to separate the user interface from the business logic.


Order | Workflow | Complete
:-------------: | :------------- | :-------------: |
1 | *Start by creating basic functions and back-end logic to solve the problem*: Using HTML and JS and jQuery. | --
2a | *Refactor by putting program functions into their own files*: Use additional `.js` files. | --
2b | *Use separate file for front-end DOM*: Using at least 2 JavaScript files. use `...-interface.js` | --
2c | *Refactor by putting program functions into their own Node modules*: Using `exports` keyword. | --
3 | *NPM: Use npm to install necessary tools/packages (from command line):*: Node Package Manager | --
3a | *Create `package.json` `manifest` file by running npm from top lvl of project directory*: $ npm init | --
3b | *Create `gulp` JS package for development app and save it to the `package.json` `manifest`*: $ npm install gulp --save-dev | --
3c | *Download browserify package and save it to the `manifest` under devDependencies*: $ npm install browserify --save-dev | --
4 | *GITIGNORE: Create `.gitignore` file that includes `node_modules/` and `.DS_Store` in top level of the project folder*: Using Atom. | --
5 | *GULP: Create Gulpfile in top level of the project and require `gulp`*: gulpfile.js | --
5a | *Get a new package called `vinyl-source-stream` using npm*: $ npm install vinyl-source-stream --save-dev | --
5b | *Require both browserify and vinyl-source-stream in the gulpfile.js*: `var ... = require` | --
5c | *Add task to call the browserify function in the gulpfile*: `gulp.task('jsBrowserify')` | --
5d | *Run our task command in the terminal to generate the `build` folder*: `$ gulp jsBrowserify` | --
5e | *Install a new package called `gulp-concat` using npm:* $ npm install gulp-concat --save-dev | --
5f | *Createa new gulp task using `gulp.src` called `concatInterface` in the gulpfile.js:* gulp.task('concatInterface') ... gulp.src | --
5g | *Run the new version of our browserify task using gulp:*: $ gulp jsBrowserify | --
5h | *Shorten the new concatenation gulp.task even more by using a globbing pattern using* ** *(an asterisk... the wildcard symbol)*: Tell the `gulp-concat` package to concatenate and browserify all files inside of our js folder that end in the string "-interface.js". | --
5i | *Add minification to the end of our JavaScript chain using another package from npm*: $ npm install gulp-uglify --save-dev | --
5j | *Add a require statement to our `gulpfile.js`:*: js/gulpfile.js
var uglify = require('gulp-uglify'); | --
5k | *Run $ gulp minifyScripts (it will run jsBrowserify, which will run concatInterface). See that the printout works in the terminal!*: $ gulp minifyScripts | --
5l | *ENVIRONMENTAL VARIABLES: install `gulp-util` as a development dependency*: $ npm install gulp-util --save-dev | --
5m | *Require our new `gulp-util` package at the top of our gulpfile*: gulpfile.js
var utilities = require('gulp-util'); | --
5n | *Create an environment variable called production and use it inside of a new gulp task called build*: $gulp build --production | --
5o | *Add code to gulpfile.js to tell which kind of environment we are using.*: gulpfile.js ... var buildProduction = utilities.env.production; | --
5p | *Install `del` package, which stands for delete*: $ npm install del --save-dev | --
5q | *Require it at the top of the gulpfile.js*: var del = require('del'); | --



And require it at the top of our gulpfile:

gulpfile.js
var del = require('del');




5a | *Include gulp tasks to concatenate*: Using gulp. | --
5b | *Include gulp tasks to minify*: Using gulp. | --
5c | *Include gulp tasks to browserify*: Using gulp. | --
5d | *Check the code*: Using JSHint. | --
5e | *Include a functioning gulpfile with all tasks(concatenate, minify, browserify, and check your code)*: Using ?. | --
6 | *Create a clean task*: Using ?. | --
7a | *Create a build task*: Using ?. | --
7b | *Create a separate build folder for production files*: Using ?. | --
8 | *Include object declarations in the back-end file*: Using ?. | --
9 | *Include instances of each object in the front-end file*: Using ?. | --
10 | *Include manifest file with a list of npm packages*: Using ?. | --

## Setup/Installation Requirements

* _Download the repository from GitHub_
* _run $ npm install to gather the packages the program requires_
* _Visit web page_
* _Check out the viewer in multiple screen sizes_

## Known Bugs

* _none so far_

## Support and contact details

_If you run into any issues or have questions, ideas, or concerns, please feel free to contact Marty or Noah:_

* _Marty Fitchen: <a href="mailto:mfitchen@gmail.com">mfitchen@gmail.com</a>._
* _Noah Yasskin: <a href="mailto:noahyasskin@gmail.com">noahyasskin@gmail.com</a>_

## Technologies Used

* _HTML_
* _JavaScript_
* _Gulp_
* _Node_
* _Browserify_

### License

*MIT License*

Copyright (c) 2016 **_Marty Fitchen_** + **_Noah Yasskin_**

Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
