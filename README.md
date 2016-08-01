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
3 | *Use npm to install necessary tools/packages (from command line):*: Node Package Manager | --
3a | *Create `manifest` file by running npm from top lvl of project directory*: $ npm init | --
3b | *Create `gulp` JS package*: $ npm install gulp --save-dev | --

4a | *Include gulp tasks to concatenate*: Using gulp. | --
4b | *Include gulp tasks to minify*: Using gulp. | --
4c | *Include gulp tasks to browserify*: Using gulp. | --
4d | *Check the code*: Using JSHint. | --
4e | *Include a functioning gulpfile with all tasks(concatenate, minify, browserify, and check your code)*: Using ?. | --
4 | *Create a clean task*: Using ?. | --
5a | *Create a build task*: Using ?. | --
5b | *Create a separate build folder for production files*: Using ?. | --
6 | *Include object declarations in the back-end file*: Using ?. | --
7 | *Include instances of each object in the front-end file*: Using ?. | --
8 | *Include manifest file with a list of npm packages*: Using ?. | --

## Setup/Installation Requirements

* _run $ npm init_
* _Open a web browser_
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
