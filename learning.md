# Resources for Learning
A repository where I keep learning resources address. You are invited to check them out to improve your technical skills as a developer.

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

- CDN stands for Content Distribution Network. I have discovered this when learning BootStrap.
- Vanilla language = Pure language without any external libraries and frameworks
  Example: Vanilla CSS = Pure CSS without bootstrap or tailwind css and soon.
- NPM = Node Package Manager
- CJS = Common JavaScript
- ESM = ECMAScript Modules
- EJS = Embedded JavaScript
- JSON = JavaScript Object Notation. This is basically a configuration file.

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

Steps to using the command line to commit on a github repository.
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

