UNIT 14 – Sequalize Homework – Reverse Engineering Code

Instructions for unit 14 homework:

-  Reverse engineer the starter code provided and create a tutorial for the code.
-  In the Develop folder, there is starter code for a project. Begin inspecting the code to get an understanding of each file's responsibility. 
-  Then, in a Google Doc, write a tutorial explaining every file and its purpose. If one file is dependant on other files, be sure to let the user know.
-  At the end of the tutorial, add instructions for how you could now add changes to this project.
-  Following the common templates for user stories, we can frame this challenge as follows:

As a developer:

I WANT:  a walk-through of the codebase.
SO THAT I:  can use it as a starting point for a new project.

Business Context and application:

-  When joining a new team, you will be expected to inspect a lot of code that you have never seen before. 
-  Rather than having a team member explain every line for you, you will dissect the code by yourself, saving any questions for a member of your team.

Acceptance Criteria for homework:

-  GIVEN: a Node.js application using Sequelize and Passport
-  WHEN: I follow the walkthrough
-  THEN: I understand the codebase

Submission on BCS:

-  You are required to submit a link to a Google Doc explaining the application in the Develop/ folder.



How do I start using this app as the user?

** GETTING STARTED **

1.  To begin using this app, please clone this repository into your local storage.
2.  Create a MySQL db called "passport_demo".
3.  Go into the config file, open config.js and insert your personal data. For example, username and password, etc…
4.  Run terminal in the current repo and run "npm install" to install all node packages.
5.  While in terminal, run "node server.js" and you will successfully connect to server.
6.  Enjoy the app!


What does each folder and the files within each folder do exactly?


CONFIG FOLDER
    -  MIDDLEWARE FOLDER 
    
    'isAuthenticated.js' file = Restricts routes that user is not allowed to visit if not logged in. If user is logged in, it continues with request.

	'config.json' = Connection configuration to connect to server.

    'passport.js' = Contains JavaScript logic that tells passport we want to log in with an email address and password.


MODELS FOLDERS

	'index.js' = Connects to database and imports users log in data.

    'user.js' = Requires "bcrypt" for password hashing. this makes our database secure even if compromised. Here we have JS that defines what is stored on our database.


ROUTES FOLDERS

    'api-routes.js' = Contains routes for user to sign in, log out and getting users specific data to be displayed client side.

    'html-routes.js' = Routes that check if user is signed in or not, whether the user already has an account, etc… Then sends the user to the correct html page.

	'package.json' = Contains all package info, node modules used, version info etc… 

	'server.js' = Requires packages, sets up PORT, creates express and middleware, creates routes and syncs database / logs message in terminal on successful connection to server.
	
