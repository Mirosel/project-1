# Investigate and answer the questions

### I. Event Loop
    1. How it works in general
	2. How it ensures proper ordering
	3. What is non-blocking I/O
	4. How non-blocking I/O is achieved
	5. Pros and Cons of non-blocking I/O and its difference to other ones

### II. Callbacks
    1. What is callback
	2. Write an example of callback
	3. Callbacks usage (give some examples)

### III. What is Promise?
	1. Write and example of Promise
	2. Compare Promises and Callbacks, tell about difference
	3. Handling errors in Promises
	    a. How errors are handled in Promises?
	    b. Write an example of handling error in Promise
	4. What is promisify
	    a. Write an example of promisify
	    b. Write convertions promise <-> callback
	    c. Write promisify using Promise constructor
    5. What is unhandled Promise
        a. How unhandled Promises can be handled
        b. What unhandled Promise emit in older and newer version of Node.js
    6. How Promise inside Promise works?
    7. What is Promise.all / Promise.resolve /Promise.reject?
    8. When do we use Promise.all? Give an example

### IV. What is async/await and how it works
	1. Write examples of async/await
	2. Write examples of async/await usage with promises
	3. How errors are thrown and handled in async/await? examples
	4. What happens when error is thrown inside async function

### V. package.json
    1. What is package.json?
    2. What is yarn and npm?
    3. Tell about difference between dependencies and devDependencies
    4. Where packages are installed?
    5. How versions are being properly resolved among packages
        a. What is package-lock.json/yarn.lock?
        b. What is difference between package-lock.json/yarn.lock?
    6. Install dependency with yarn/npm
    7. Install devDependency with yarn/npm
    8. Uninstall dependency with yarn/npm
    9. Uninstall devDependency with yarn/npm
    8. What is scripts section in package.json?
    9. Write an example of running script from package.json


### VI. Eslint
    1. What is eslint?
    2. Reason to use eslint
    3. Create an example project with eslint
    4. Add some rules
    5. Add script to package.json to lint all files in project
    6. Add script to package.json to fix all fixable errors in project
    7. Enable eslint in WebStorm (Show whether it works)

### VII. Packages
    1. How packages are resolved?
    2. What are node_modules?
    3. How package.json is connected to node_modules?
    4. How module can be created? Example
    5. Difference between
             `require('aaa')`
         and `require('./aaa')`
         and `require('./aaa.js')`
    6. What is index.js/index.ts
        a. How index can be used? Example
        b. What is re-export? Example
        c. How directory can be imported as package?


### VIII.General
    1. URL
        a. What is query? Example
        b. What is param? Example
        c. What is hash? Example
    2. REST API
       a. What is REST?
       b. Tell about every REST method (GET, POST, PUT, DELETE, HEAD ...etc)
       c. Difference between GET and POST/PUT
       d. When each method should be used?
       e. status codes: 404, 500, 503, 400, 403, 200, 401

### IX. MVC
    1. What is M in MVC? Describe the M
    2. What is V in MVC? Describe the V
    3. What is C in MVC? Describe the C
    4. What should/n't controller do?

### X. Patterns
    1. Tell about Repository pattern. How it works in general? Reason to use
    2. Tell about Service pattern. How it works in general? Reason to use
    3. Tell difference between Service and Controller
    4. Tell difference between Respository and Service
    5. When Service/Respository should be used?

### XI. Express
    1. What is RequestHandler? example
    2. What is Handler? Difference Handler <--> RequestHandler
    3. What is Route? example
    4. What is Router? example
        a. Reasons to use Router?
    5. What is Middleware? example
        a. When midlleware is used? example
        b. What can be achieved using middleware? example
    6. What is ErrorRequestHandler? example
    7. What is `next` function in RequestHandler
    8. May async function be used as RequestHandler
        a. Write a converter that converts callback RequestHandler to async RequestHandler

### XII. import/export
    1. What is common.js?
    2. What is `require`?
    3. What are ECMASript modules?
    4. Difference between *.js and *.mjs files
    5. How modules can be enabled?
    6. What is named export?
    7. What is default export?
    8. Difference between named and default export? May them be combined?
    9. Why it's better to not use default export
    10. Write an example of named/default export from file using common.js
    11. Write an example of named/default export from  file usinf ECMA modules

### XIII. Typescript
    1. What is Typescript
    2. What are @types/* packages
    3. May @types/* packages be installed in Javascript project
        a. Why it's better install @types/* packages?
        b. When @types/* packages should not be installed

# Project

* Packages that may be used
    * pug
    * moment
    * express
    * sqlite3
    * eslint
    * pug
    * @hapi/joi
    * @hapi/boom
* Project should be configured with eslint
* Project should use MVC
* Use `@hapi/joi` to validate objects
* Use `@hapi/boom` in controllers
* User `pug` for html rendering
* You may use any style framework, but pages should be responsive and good looking
* Use `moment` to handle dates and timestamps, use format `YYYY-MM-DD HH:mm:ss`
* Project should use sqllite file based db
* Use Node 14

### Structure of project
- SimpleProject
    - src/
        - middlewares/
        - models/
        - views/
        - controllers/
        - repositories/
        - services/
        - schemas/
        - toolkit/ <-- helpers and utils
        - routes.mjs <-- Put routing here
        - server.mjs <-- Server initialization
        - index.mjs <-- File that starts application
