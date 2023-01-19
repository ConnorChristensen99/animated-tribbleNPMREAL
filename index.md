# NPM Documentation
*****

### 1. What is NPM? What does it do? Why is it an important tool?
NPM stands for "Node Package Manager". At its core, it is a library for JS software packages with command line tools to help as you are developing. This is an extremely important tool as it allows you to install packages and manage their dependencies all from the ease of a command line. Due to it being open-sourced, it is also a great place for developers to create and share software packages. 

### 2. What problems does NPM Solve?
NPM solves the problem of having you or others work on a project with dependencies later down the line, as it is an easy npm install command to get up to speed. On top of this, it easily manages all of the libraries you have rather than having to download them by hand and move them into the correct directories and THEN make sure that the version of the project and all of the now installed dependencies are up to date and on the same page. 

### 3. Describe the 3 main parts of NPM.
*The Website* - using npmjs.com you are able to set up a profile and organizations as well as look for packages. <br/>
*The Command Line Interface (CLI)* - This runs from a terminal and is usually how you will interact with NPM. <br/>
*The Registry* - This is a large database, that is public as NPM is an open-source project,  where you can see all of the different JS software and the meta-information with it.

### 4. What is the package.json file?
This is the heart and soul of any project as it is a file that contains the metadata about the project in regards to NPM. When sharing a project or getting started on one again, anything in this file will get you back up to speed as it has attributes that npm will use to install the necessary dependencies and run any scripts you may have. 

### 5. What is the scripts section of the package.json file? How do you use it? What are the default commands, and how do you use your own?
A script here is simply an easy way to bundle common and annoying commands or tasks that may have to be run multiple times. To use a script, you need to define it in the package.json file along with the command you want to run when you call the script. To run said script, you need to use the command `npm run <NAME_OF_SCRIPT>`. 
Scripts can either be installed or created on your own by the following: <br/>

"scripts": {<br/>
  "name_of_script_here": "command_to_be_run" <br/>
  } 


### 6. What are dependencies? What does this section define? What are dev dependencies? Why is it important to define dev dependencies vs dependencies?
Dependencies are another package that comes along with an NPM install when you get a library automatically; they contain the references that your library uses to function properly. A dev dependencies are something that the developer relies on when developing the project and testing it locally. The dev dependencies are not necessarily going to be needed at launch, just to test or while working on the project. This is important as it could be devastating to have the test going well and then lose the necessary dependencies needed to keep the program alive. 

### 7. How do you install dependencies? Where do dependencies get installed?
When using NPM to install a package, it should automatically install both the dev dependencies and regular necessary dependencies. These are then stored in the `node_modules` folder.

### 8. When running scripts with NPM, where does NPM look (path) for the dependencies of those scripts?
When NPM looks for the dependencies of a certain script, it looks for them in the `node_modules` folder.

### 9. Name 3 NPM commands, and why they are important.
`npm install` - This command is important as it installs packages into the package.json file and allows you to access the power of npm. <br/>
`npm start` - This command is used when you are wanting to run the server command to start a project. This specifically will run a command that is defined in the start property of the script. If nothing is there then it will auto run that start server command.<br/>
`npm init` - When starting a project this command is extremely important as it initializes your project and creates a package.json file in the current directory you are in.    <br/>
