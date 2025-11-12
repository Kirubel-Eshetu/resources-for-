# Resources for Learning
🗃️ A repository where I keep learning resources address. You are invited to check them out to improve your technical skills as a developer.

## From the course "The Complete 2024 Web Development Bootcamp" taught by Dr. Angela Lu
### For responsiveness using Media Quieries
- Mobile Devices: 319px - 480px
- iPads and Tablets: 482px - 1200px
- Laptops: 1201px - 1600px
- Desktops: 1601px and more.

### For learning Flex-box
- <a href = "https://appbrewery.github.io/flexboxfroggy/" style="text-decoration:none;"> Flex box froggy game </a>

### For learning Grid-box
- <a href = "https://appbrewery.github.io/gridgarden/" style="text-decoration:none;"> Grid Garden Game </a>

### For minifying code
- <a href = "https://www.minifier.org/"> Minify your code </a>
- Minifing means reducing the size of your code through space and comment removal.

### Short Notes
- Higher order functions are functions that can take other functions as inputs.
- Node is not a JavaScript framework, rather Node is a runtime environment. Node allows us to run JS on a computer and not just limited on the computer.

### Fun
- Would like to have fun with the fake hacker typer? then checkout <a href = "https://hackertyper.com/"> hackertyper </a>

### Learn Enough Command Line to be Dangerous
- Visit the <a href = "https://www.learnenough.com/command-line-tutorial"> learn enough </a> website

### Common words and Abbrevations
- CDN = Content Distribution Network. Discovered this when learning BootStrap.
- Vanilla language = Pure language without any external libraries and frameworks
  Example: Vanilla CSS = Pure CSS without bootstrap or tailwind css and soon.
- NPM = Node Package Manager
- CJS = Common JavaScript
- ESM = ECMAScript Module --> It is a library. ECMAScript is the modern name for JavaScript.
- EJS = Embedded JavaScript
- JSON = JavaScript Object Notation. This is basically a configuration file.
- ARIA = Accessible Rich Internet Applications

### HTTP return codes cheat sheet
- GET => Request resource.
- POST => Sending resource.
- PUT => Update by replacing resource.
- PATCH => Update by patching up a resource.
- DELETE => Deleting a resource.
- 1xx => Hold on
- 2xx => Here you go
- 3xx => Go away
- 4xx => You (the user) screwed up 
- 5xx => I (the server) screwed up

### Version control using git and GitHub
- Steps to using the command line to commit on a github repository.

#### Creating Local Repostitory
      1. git init 
      2. git add example1.example1 example2.example2
      3. git commit -m "Your commit message here"

### status and rollback
      - git status --> to check the status 
      - git log --> to get information about recent commits made.
      - git diff filename --> check the difference of a file from the original version
      - git checkout filename --> rollback a file to it's last version

#### Creating Remote Repostirory 
      1. git remote add origin github_repository_url
      2. git branch -M main --> Change the deafult branch to main ( the code is going to be pushed here)
      3. git push -u origin main --> Push the code from local to remote repository
      
#### Pull requests
  - Pull Requests: Create pull requests to propose changes and request code reviews before merging.

      1. git pull --> pull and merge form remote to local repositories
      2. git pull origin main --allow-unrelated-histories --> pull form remote repository and merge it by allowing unrelated histories.

 #### git branching
      1. git branch <branch-name> -> to create a new branch.
      2. git checkout <branch-name> -> to switch between branches.
      3. git merge <branch-name> -> to combine changes from one branch into another
      
#### Git Cloning
      git clone url

#### Update Git Remote URL
      - git remote -v - Check repository’s remote URL
      - git remote set-url origin https://<your-username>:<your-token>@github.com/repository-url.git - If it’s using HTTPS, update the remote to include your username and PAT.

### APIs
- https://www.bored-api.appbrewery.com/endpoint?query=value&query2=value2. bored-api.appbrewery.com ---> base URL   endpoint ---> endpoint  ?query=value&query2=value2 ---> query

### JSON
- To see a humanoid version of JSON ---> jsonviewer.stack.hu
- A password decoding website ---> base64decode.org
- JSON visualizer --> <a href = "https://jsonviewer.stack.hu/">jsonviewer.stack.hu</a>

### Angular
- Angular supports MVC architecture. MVC architecture allows developers to separate thier code into 3 distinct parts, namely Model, View and Controller.

#### Collaboration addresses
- https://github.com/MunGell/awesome-for-beginners.git

#### Random Image Resource
- https://picsum.photos/

### React
- React is a lightweight library from Facebook <br />
    - Helps you develop large-scale web applications. <br />
    - Give you a logical way to construct your UI code. <br />

- React allows you to create apps for <br />
    - Web browsers (via Reactjs) <br />
    - iOS/ Android native devices (via React Native) <br />

- Most browsers also support an extension callec React Developer Tools <br />
    - Helps you understand the hierarchy of elements in your UI

- React has quite a small number of libraries. <br />

- There are two ways to incorportate these libraries in your web app: <br />
    - Download the libraries directly into your app at run-time <br />
    - Pre-package the libraries into your app at dev-time

- A React web app has a single, top-level HTML element into which React will render the UI.
- You typically define it as a <div> like this:
    <div id="root"></div>
- Give the element a suitable id
    - You'll render React content here.
- React:- class enables you to create element objects.
- createRoot:- a function that creates a root, into which you render your React content.

#### Understanding the DOM (Document Object Model)
- Browsers maintain an in-memory tree of objects called the Document Object Model (DOM)
    - The DOM tree represents the contents of the web page.
- Traditionally, you would use the DOM API to modify the contents of the web page programmatically
    - Create new elements
    - Append child elements
    - Set attributes
    - Etc..

##### Problems with Manipulating the DOM Directly
- Manipulating the DOM directly is tedious
    - You have to write a lot of code to achieve anything
    - This is why libraries such as jQuery became popular
- Manipulating the DOM directly is also quite slow
    - When you modify any content ini the DOM, the browser re-renders a large portion of the DOM tree.

#### Understanding the React Virtual DOM
- React introduces the concept of the virtual DOM:
    - A bunch of element objects that are going to be rendered.
    - A copy of the browser's real DOM.
    - Contains lightweight copies of objects in the real DOM.
    - React only re-renders nodes that have changed.
    
##### Viewing the Virtual DOM
- You can view the virtual DOM in a browser, by using React Developer Tools in Chrome...
    - Open a React web page in the browser
    - Show the DevTools window (F12)
    - Click the Components tab
    - In the Serach window, click the Settings cog
    - In the popup window, select the Components tab
    - Deselect the "Hide components where" option

#### Mapping Data to Elements
- You can use map() to map array items to React elements. <br />
    someArray.map((arrayItem, index) => React.createElement(htmlElement, htmlProperties, htmlContent)) <br />
    - index can sometimes be written as idx.
- map () takes a lambda parameter
    - The lambda receives 2 args - (array item, index).
    - The lambda creates and returns a React element.

#### How to Define Components in React
- There are two ways to develop components in React...
    - Via classes and inheritance
    - Via functional components

##### Introducting Functional Componenets
- You can define a component as a function, rather than as a class.
- Benefits of functional components:
    - Simpler syntax than class components
    - Support modern features in the React library
- To define a functional component:
    - Just define a function (name must start with a capital letter)
    - In the function, create and return the component's UI
###### Defining Functional Components
- Here's the functional component for products data:
    function ProductList() {
        return React.createElement("p", null, "Products data list")
    }
- Whenever you see a function in React capitalized, it is a component which means it returns a subset of the virtual DOM.

#### What is Destructuring?
- Destructuring is a language feature in ECMAScript 2015. The offical name of JavaScript is ECMAScript.
    - Extracts properites from an object into a separate variables.
    - For Example:
    let object = {"fname": "Kirubel", "car": "Mustang", "hobbie", "Golf" };
    let {fname, hobbie } = object;

    console.log(`Hi this is ${fname}. My hobbie is ${hobbie}`)

#### Introducing JSX
- React supports a lightweight syntax called JSX.
    - A combination of JavaScript and XML.
    - Enbales you to create React elements concisely via XML.
- Example:
    const messiah = <h1>Jesus is Lord and the messiah.</h1>
    - on the above JSX code, const messiah is JavaScript. While <h1>Jesus is Lord and the messiah.</h1> is an XML.
##### Transpiling (Compiling) JSX
- Browsers don't understand JSX syntax directly.
    - JSX syntax must be transpiled into "pure" React.
- You can use the Babel transpiler to do this.
    1. Add a <script> tag to download the Babel transplier
    2. Embed JSX code inside <script type = "text/babel">
        <script src="..URL for Babel transpiler..."></script>
        <script type="text/babel"...>
            Some JSX script here. (Don't hack with them :)
        </script>
##### JSX Content
- JSX elements can contain:
    - Text content
    - JavaScript expressions
    - Other nested elements, as deeply nested as you like

#### Ways to start with React
    1. npx create-react-app your-react-app-name
    2. cd your-react-app-name
    3. npm start
1. Create a new react project.
2. Change the directory into that project folder.
3. Start the server.

#### React's Map, Reduce, Find and FindIndex functions.
- There are three ways to execute these functions.
##### Map Function
const numbers = [5, 10, 15, 20, 25, 30];

1. function square(num) {
  return x * x;
};
- const squareNum = numbers.map(square);
- console.log(squareNum);

2. const squareNum = numbers.map(function (num) {
  return x * x;
});  
- console.log(squareNum);

3. const squareNum = numbers.map((num) => x*x);
- console.log(squareNum);

##### Reduce Function

const numbers = [5, 10, 15, 20, 25, 30];

1. function accNum(accumulator, currentNumber){
      return accumlator + currentNumber;
   };
- const accumulatedNum = numbers.reduce(accNum);
- console.log(accumatedNum);

2. const accumulatedNum = number.reduce(function (accumulator, currentNumber){
      return accumulator + currentNumber;
   });
- console.log(accumulatedNum);

3. const accumulatedNum = number.reduce((accumulator, currentNumber) => accumulator + currentNumber);
- console.log(accumlatedNum); //For checking the output
   
#### Find Function

const numbers = [5, 10, 15, 20, 25, 30];

1. function findNum(num){
    return num < 15;
   }
- const findNumber = numbers.find(findNum);
- console.log(findNumber);  //For checking the output

2. const findNumber = numbers.find(function (num) {
   return num < 15;
   });
- console.log(findNumber);

3. const findNumber = numbers.find((num) => num<15);
- console.log(findNumber);

##### FindIndex Function

- const numbers = [5, 10, 15, 20, 25, 30];

1. function findNum(num){
    return num < 15;
   }
- const findNumber = numbers.findIndex(findNum);
- console.log(findNumber);  //For checking the output

2. const findNumber = numbers.findIndex(function (num) {
   return num < 15;
   });
- console.log(findNumber);

3. const findNumber = numbers.findIndex((num) => num<15);
- console.log(findNumber);

### Starting Servers of different Frameworks

    1. node entryfilename.js / nodemon entryfilename.js (If you have nodemon installed)  => For node, Express
    2. npm start  => For react
    3. ng serve   => For Angular

## MongoDB
- A collection is a group of documents and a database is a group of collections.

## Docker
- You can build an image using the following docker build command via a CLI in your project folder.

      docker build -t welcome-to-docker .

# MongoDB course by Max Schwezner
### Databases, Collections and Documents
- A Database holds multiple Collections where each collection can then hold multiple Documents.
- Databases and Collections are created "lazily" (i.e. when a Document is inserted).
- A Document can't directly be inserted into a Database, you need to use a Collection!
  
### Document Structure
- Each document needs a unique ID ( and gets one by default)
- You may have embedded documents and array fields.
- MongoDB doesn't use JSON but BSON (Binary JSON). We write a JSON file and MongoDB Drivers converts that JSON to BSON.

### Some commands
      use databaseName -> create a new database
      db.dropDatabase() -> Delete a database
      mongoimport filename -d databaseName -c collectionName --jsonArray
      db.createUser({user: "username", pwd: "password', roles: ["readWrite]}) -> Create a user
      db.getUser("username") -> get information about a user

### Resources
Learn more about the MongoDB Drivers: https://docs.mongodb.com/ecosystem/drivers/
Dive into the official Getting Started Docs: https://docs.mongodb.com/manual/tutorial/getting-started/

# JWT (JSON Web Token) Generation
- Using Node.js => node -e "console.log('JWT_SECRET=' + require('crypto').randomBytes(64).toString('hex'))"
- Using OpenSSL (Secure Sockets Layer) => openssl rand -hex 64

# Running HTML file from the termial
## 1. Using Python (Recommended)
    cd project_folder
    python -m http.server 2300
- Then open your browser and go to: http://localhost:8000
  
## 2. Using Node.js (if you have it installed)
    npm install -g http-server
    cd project_folder
    http-server
## 3. Using PHP 
    cd project_folder
    php -S localhost: 2300

## 4. Direct File Opening (Limited)
### On Windows
    start index.html

### On macOS
    open index.html

### On Linux
    xdg-open index.html
    
# Running app
1. React app
2. Angular app
3. Node app
4. Nextjs app => npm run dev

## From the course "Junior Backend Development" through Gebeya by Ismael Kedir

### Concepts
#### What is an ORM (Object-Relational-Mapping)
- An ORM like Prisma is a tool that helps us interact with a relational database using code instead
of writing SQL queries directly. <br />
- Prisma also supports MongoDB, but its feature set is more limited for NoSQL databases. It's still
a great option for basic operations, but Object Document Mappings (ODMs) like Mongoose are more specialized for MongoDB-specific features like embedded documents.

#### Middleware and Routing

- Middlewares are functions that run before the final request handler, modifying the request, response or both. <br />
- Routing defines how requests are handled for specific endpoints and HTTP methods. <br />
- Router-level middleware: Allows for more modular and scalable code organization. <br />
- Error-handling middleware ensures that your app can gracefully respond to issues and provide userful feedback to users. <br />

#### Logging and Monitoring

- Logging and monitoring provide insights into the application's behavior and performance, helping
  track down issues in production. <br />
- Logging: Helps track events and errors that occur while the application is running. <br />
- Monitoring: Helps track the health and performance of your application over time. Example tools: 
  PM2


#### Depolyment and DevOps Basics
##### Environment Configuration

- Environment Conifguration is all about preparing your application to run seamlessly accross different environemnts-development, testing and production. It ensures your app can run in different environments

    - Development Environment: Where you write and test your code locally.
    - Testing Environment: Used for quality assurance and running automated tests.
    - Production Environment: Where your application serves real users.

##### Build and Depolyment Pipelines

- A build and depolyment pipeline automates the process of preparing and pushing your application to production.

- Build: Compiles TypeScript to JavaScript and packages your app for depolyment. <br />
- Test: Runs automated tests to catch bugs before deployment. <br />
- Deploy: Pushes the code to a live environment, making it accessible to users.

##### Continuous Integration and Continuous Deployment (CI/CD)

- Continuous Integration/Continuous Deployment(CI/CD) helps automate the entire development process, from testing to deployment.

###### Continuous Integration (CI)
 - Continuous Integration is a practice where developers frequently push code to a shared repository. <br />
 - Automated tests run on every push to ensure that new changes don't break exisiting code. <br />
 - CI tools: GitHub Actions, GitLab CI, Travis CI, CircleCI.

##### Continuous Depolyment (CD)
- Continuous Deployment automates the depolyment of code after it passes all the tests in the CI pipeline. <br />
- With CD, once your code passes tests, it automatically gets deployed to production (or desired environment)

### Recommended Resources
1. MDN Web Docs- Backend Development - A solid resource for understanding backend concepts.
   https://developer.mozilla.org/en-US/docs/Learn/Server-side

2. Backend Roadmap
   https://roadmap.sh/backend

3. How APIs Work (Postman Blog)
   A clear, beginner-focused explanation of APIs and how they enable communication between systems.
   https://www.postman.com/what-is-an-api

4. Introduction to Cloud Computing by AWS
   A beginner-friendly guide to understanding the basics of cloud computing, ideal for grasping the concept of scalable server infrastructure.
   https://aws.amazon.com/what-is-cloud-computing

5. What is a database in under 4 minutes - Video on YouTube 
   https://www.youtube.com/watch?v=Tklt3WKK-ZY&ab_channel=LinuxAcadamy

6. JavaScript Guide | MDN
   https://developer.mozilla.org/en-US/docs/Web/JavaScript

7. TypeScript 5 fundamentals
   https://app.pluralsight.com/libraray/courses/typescript-5-fundamentals/table-of-contents

8. TypeScript on Exercism - Explore and get fluent in Typescript
   https://execism.org/tracks/typescript

9. Object-oriented programming - Learn web development | MDN
   https://developer.mozilla.org/en-US/docs/Learn/JavaScript...

10. Pro Git-Book
    https://git-scm.com/book/en/v2

11. Git Guides by GitHub
    https://github.com/git-guides

12. Oh My Git - A game-like tool to practice Git commands in an interactive and fun way.
    https://ohmygit.org

#### REST Clients

- REST APIs uses multiple, distinct endpoints for each resource, returning pre-defined data structures.
- GraphQL allows clients to request only the specific data they need from a single, unified endpoint.

13. Postman -> https://www.postman.com

14. Insomnia -> https://www.insomnia.rest

15. ApiDog -> https://app.apidog.com

16. Firecamp -> https://firecamp.dev

17. HTTP -> MDN Web Docs
    https://developer.mozilla.og/en-US/docs/Web/HTTP

18. RestApiTutorial Website
    https://www.restapitutorial.com/

#### Building Your First Web Application

19. Express.js Documentation
    https://expressjs.com

20. How to set up TypeScript with Node.js and Express - Article by LogRocket
    https://blog.logrocket.com/how-to-set-up-node-typescript-express

21. REST API Tutorial
    https://resfulapi.net

#### Database Fundamentals

22. SQL Tutorial by W3Schools
    https://www.w3schools.com/sql

23. What is NoSQL? - Resource by MongoDB
    https://www.mongodb.com/resources/basics/databases/nosql-explained

#### Integrating Databases with Your Application

24. Building a modern backend with TypeScript, PostgreSQL and Prisma
    https://www.prisma.io/blog/series/modern-backend-bdes2ps5kibb

25. Database integration Guide by Express.js
    https://expresis.com/en/guide/database-integration.html

26. FreeCodeCamp's CRUD API Tutorial with Node.Js, Express, MongoDB | YouTube
    https://www.youtube.com/watch?v=7UQPve99r4

27. Prisma Documentation
    https://www.prisma.io/docs

#### Middleware and Routing

25. Express.js Middleware Documentation
    https://expressjs.com/en/guide/using-middleware.html

26. Express.js Routing Documentation
    https://expresjs.com/en/guide/routing.html

#### Web Application Security Basics

27. JWT.io - Learn more about JSON Web Tokens and how they work.
    https://jwt.io

28. Passport.js Documentation
    https://www.passportjs.org

#### Testing and Debugging

29. Jest Documentation
    https://jestjs.io/docs/getting-started

30. Debugging Node.js
    https://nodejs.org/en/learn/getting-started/debugging

#### Deployment and DevOps Basics
31. Node.js Best Practices
    https://github.com/goldbergyoni/nodebestpractices
32. Docker for Beginners - Learn to build and deploy your applications easily to the cloud with Docker
    https://docker-curriculum.com

## From the course "Tailwind CSS From Scratch - Learn by Building Projects" through O'REILLY by Brad Traversy
### Introduction
#### What is Tailwind CSS
- Tailwind is a CSS framework that uses low-level "utility" classes to create layouts. This is known as a utility-first framework.
- Traditional CSS frameworks like Bootstrap use classes that are directly correlated to components (eg. Alerts, Navbars). Tailwind uses
classes as utilities to put together to build your own custom components.
- Utility classes are simple HTML classes typically scoped to a single and specific CSS property.

## AJAX
- AJAX stands for Asynchronous JavaScript and XML. <br />
- It’s a technique that allows web pages to send and receive data from a server asynchronously — without reloading or refreshing the entire page.


