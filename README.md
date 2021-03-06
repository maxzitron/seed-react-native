# seed-react-native
A generator for ready-to-implement react-native project. After initiate a new project all required depedencies will also download and automatically config.
- React Native
- Redux
- Yeoman

## Dependencies

- [NodeJs](http://nodejs.org/) : I suggest you install this via [Node Version Manager NVM](https://github.com/creationix/nvm)

    This project depends on Node versions greater than v4, use nvm to install and setup open up the command line and run
    
    ```bash
    $ nvm install 4.x.x
    ```
    
    Next simply switch to node v4:
    
    ```bash
    $ nvm use 4.x.x
    ```
    
    This will change your current terminal session to use 4.0.0. If you want to use it permanently run:
    
    ```bash
    $ nvm alias default 4.x.x
    ```
  
- NPM - NPM may or may not have been installed with Node. Try:

    ```bash
	$ npm
	```
		
    If you get a "not found" error, run this:
		
	```bash
	$ curl -L https://npmjs.org/install.sh | sh
	```

- React Native Command Line Tools - This is a crucial Node.js module that make seed-react-native working,

	```bash
	$ npm install -g react-native-cli
	```
	If you have some error related to permission, please run
	
	```bash
	sudo npm install -g react-native-cli
	```

## Getting Started Instructions

To create a new seed-react-project, CD into your target folder and run init command

    $ seed-react-native init <Project Name>

seed-react-native will first initiate a new react native project based on your given name and then scafold your project. This process may take a bit of time.

After all done, the project folder will be created based on the given project name.

To start an application, CD into the project folder and run

    $ react-native run-ios
    
for iOS application
    
    $ react-native run-android
    
for Android application

## Project Strucuture
Below is the applcation structure:

	- local-cli/ ---| <!-- Contains files for building project structure -->
			- generator/ <!-- Contains all project template file -->
			- cli.js <!-- Main code for scafolding a new project by useing [Yeoman](http://yeoman.io/) -->
	- index.js <!-- Main Node.js script for recieving command from CLI -->
	- package.json
	- processes.json
	- README.md
