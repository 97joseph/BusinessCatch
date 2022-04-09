# BusinessCatch
 Call center for business using MVC in ionic
 
  
Goal  
Design a simple, visually pleasant, functional and responsive, mobile app that performs a useful (set of) function(s). 
You should use (and demonstrate your knowledge/understanding of): HTML5, CSS, JavaScript, AngularJS, Ionic Framework, and Cordova.
  
Milestone 1: Set up and workflow 	 
The goal of Milestone 1 is to demonstrate that you got the entire Ionic mobile app development workflow working properly and that you can make trivial modifications to a simple sample app. 
 	 
Recommended Procedure: 	 	 
Steps below are based on the “Ionic 4 Crash Course” (YouTube video: 
https://www.youtube.com/watch?v=YwSzqeBchEc&feature=youtu.be) 
  
1.	Go to http://ionicframework.com/ and click on the 'Get started' button. 	 
2.	Download ( from https://nodejs.org/en/ ) and install Node.js (LTS version) and npm. At the end of the installation process you should see a dialog box like this. Make a note of the directories where node.js and npm have been installed. 	 
	  	 
3.	Install the Ionic framework (fix possible warnings; $ is the prompt, no need to type ‘sudo’ if on Windows):   
$ sudo npm install -g @ionic/cli     
npm WARN ws@7.2.3 requires a peer of utf-8-validate@^5.0.2 but none is installed. You must install peer dependencies yourself. 
 
$ sudo npm install -g npm-install-peers 
  
4.	Create a new Ionic app using a blank template: 	 
$ ionic start myapp blank –-type=angular --capacitor $ cd myapp  
$ ionic lab //runs the app in a device simulation environment  
	  	 	//accept to install ionic lab 
Alternative: you can run the app full screen in the default browser on your desktop by typing 
$ ionic serve 
 	 	 
5.	You should see a "welcome" app on your browser window, like this:  
	  	 
6.	Explore the directory structure of the Ionic project, using your favorite editor – Atom or Brackets are good options.  
7.	Open the folder where the Ionic project resides in your machine, locate the home.page.html file under the 'src/app/home’ folder, make a minor change and save it, and watch the change happen ‘live’ on Ionic Lab. (Important Note: the Brackets browser sync does not render the Ionic app gracefully. You will need to run your app with Ionic lab or Ionic serve. Changes that you make to the app will sync when you save them, whichever editor you use) 	 
8.	Customize the contents of this basic app to display a different text and title. 
9.	Follow along the “Ionic 4 Crash Course” YouTube tutorial and add another page and navigation buttons to your app. Also see the Ionic example from class (files in Canvas). Use the following 
command in your application directory to generate a new page component  
$ ionic generate page mypage  
10.	(OPTIONAL) create and explore the structure of the getting started sample apps using the tabs or side menu templates. (https://ionicframework.com/getting-started#cli) 
 
11.	(OPTIONAL) create and explore the structure of more complex sample templates using the conference template. 
  
12.	(OPTIONAL) Build and run the app using a native Simulator (e.g., iOS Simulator for Mac OSX or Android simulator).  
i.	If not already installed, install iOS emulate/run functionality: Click on the ‘Install’ button next to the iOS platform icon on Ionic Lab. 	 
ii.	Run these commands on the Terminal (address build process errors; Google search fixes on the web): 	 	 
$ ionic build 
$ npx cap add ios 
	$ npx cap open ios 	 
	• 	Install Android emulate/run functionality by: 	 
i. Click the ‘Install’ button next to the Android platform icon on Ionic Lab. ii. Running this command on the Terminal: 	 	 
$ npx cap add android 
$ npx cap open android  
• 	Search the web for the error string, usually find solution in stackoverflow.com 
	i. 	An unhandled exception occurred: [BABEL] 
/Users/mpm/IonicProjects/m2020-ex4-migrated/www/stencil-ionapp_8-md-entry-js-es2015.js: Could not find plugin "proposalnumeric-separator”.  
1	Add  "resolutions": { "@babel/preset-env": "7.5.5" }, to package.json. 
2	Run npx npm-force-resolutions 3 Run npm install . 
4 Run build to build your project ii. npm WARN ws@7.2.3 requires a peer of bufferutil@^4.0.1 but 
none is installed. You must install peer dependencies yourself. 
1 sudo npm install -g npm-install-peers 
13.	BONUS: Make additional content customizations (e.g., add images, colors, links, buttons, and other components). 	 	 
 
 	 
  
Milestone 2: First ionic app
 
The goal of Milestone 2 is to demonstrate that you managed to implement an actual app using the
Ionic mobile app framework.	 	 
Recommended Procedure: 	 
Steps below are based on the “Ionic 2 by Example:  Creating Your First Ionic App” (YouTube video:  https://youtu.be/qdeD9rYlBU4 ). Note that Ionic is presently at version 5, and directory structures have changed. This is for better clarity but may still be confusing the beginner. The exercise is valuable, and a working example is provided in Canvas. 
  
11.	Go to http://ionicframework.com/docs/	and keep a tab open on that page. 	 
12.	Go to your working directory on terminal and create a new app, as follows:  
$ ionic start love-calculator blank -–type=angular --capacitor  
13.	Go to the app directory and open its folder structure using your favorite editor, e.g. Atom: 	 
$ cd love-calculator  $ atom .  
14.	Run the app using the syntax below: 
$ ionic serve  
15.	You should see a blank app screen like this:  
   
16.	Explore the directory structure of the Ionic project, using your favorite editor (follow instructions in the video). 	 
17.	Open the folder where the Ionic project resides in your machine, locate the home.html file under the 'src/app/home' folder, make a change to its title, save the file, and watch the change happen ‘live’ on the browser window ( http://localhost:8100/ ). 	 
18.	Customize the app1 (main screen, CSS tweaks, colors, font size, etc.) following the instructions in the video – from 11:25 until 28:58. 	 
19.	Customize the app (property bindings, score calculation, etc.) following the instructions in the video – from 29:05 until 40:24. 	 
20.	Customize the app (icons and final touches) following the instructions in the video – from 40:25 until the end.  	 
                                                                                                                                                 
  
1 You	can	see	the	code	changes	made	at	each	step	as	Git	commits	in	this	repository:	https://github.com/mirkonasato/ionic2-by-example/commits/love-calculator		 
  
Milestone 3:  Your app 	 
    
The goal of Milestone 3 is to demonstrate the process of creating a simple mobile app using Ionic. 
Recommended Procedure: 	 
  
25.	Start from a sample app (such as Love Calculator in Milestone 2 or the TO DO list at  https://www.joshmorony.com/build-a-todo-app-from-scratch-with-ionic-2-videotutorial/ ).  
26.	Create a baseline app containing a working solution. 	 
27.	Improve / modify the baseline app in a meaningful way, focusing on one aspect at a time (see grading rubric at the end of this document). Keep it simple. 	 
28.	Test your app after every significant change / addition. 	 
29.	Once you’ve reached a point where your app is complete and fully functional in the device / simulator of your choice (iOS and/or Android), prepare the final package (single zip, all that is needed, and nothing else).  
30.	Prepare a detailed report explaining the main building blocks of the solution, the libraries used in the final design, as well as all the relevant technical and organizational aspects. (See additional hints on what to include in the report on the next page.)  
31.	Submit the final package via Canvas.  Minimum requirements:  
•	Your app must be your own work. If you use any existing app, template, library, site, textbook example or any other source along the way, please make a note of it in your report.  
•	Your app must be fully functional. 	 
•	Your app must run in at least one (iOS or Android) simulator  
  
Deliverables 
•	A single zip file containing all files (.html, .css, .jpg, .js, etc.) necessary to run your app in a device simulator and your report (see below). 	 
•	A report (5-20 pages) describing any relevant aspect that I cannot tell just by looking at the code or playing with the app. I’m particularly interested in reading about: 	 
o	The Ionic Framework learning curve 	 
o	Which design decisions your team had to make and why you chose a particular course of action for each of them 	 
o	Which simulators / devices (phones/tablets) you tested your app on  o How close is this prototype to the “final app” that your team will present  
(together with the business plan) at the end of the term o Which libraries  plugins, editors, IDEs, tools, etc. you used o Which tasks were more time-consuming 
o	How was the workload divided among team members. Make sure you attach the group contribution form signed by all team members with your project submission 
 	 
 	 

