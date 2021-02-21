## Please, note that this repositoty is under construction!

# Angular-Bootstrap!

Contents of this repo:

1.- How to create an Angular app.<br>
2.- How to deploy an Angular app into the remote server (to Firebase, in this case).<br>
3.- Some examples of Angular (+Bootstrap) apps.

## 1.- How to create an Angular app.

1. Install node.js // used for installing the Angular-CLI. (Follow https://nodejs.org/en/ instructions) <br>
After that, we can run npm (Node Package Manager) commands in our system.
	
2. Install Angular-CLI // official Angular line command. [sudo] could be required in Mac/Linux systems <br>
After that, we can run ng commands, such as create a new Angular app.

		> [sudo] npm install -g @angular/cli@latest

3. Create a new app.<br>
After that, an Angular app is created, we can edit it (with VSCode or any other editor).
		
		> ng new angular-hello-world

4. To run locally our app, we have to go inside the angular-hello-world folder and run <br>
Next command compiles our app and deployes it to the local server, port 4200.
	
		> ng serve

5. View app in local browser (URL is showed by ng server when compile is finished) <br>
	
		> URL = http://localhost:4200/
	
6. Prepare the app to be deployed to the remote server. Inside the angular-hello-world folder <br>

		> ng build --prod  // this creates a dist folder!
	
7. A new folder is created (folder = dist/angular-hello-world). That folder will be used to deploy to the remote server.


## 2.- How to deploy an Angular app into the remote server.

8. Choose the server. On my case, I choosed Firebase (free) hosting. After creating our account on Firebase we need to create a new Project.
We do that in Firebase's Console accepting the default settings. Pretty straightfordward. Project's name could be the same as the Angular (angular-hello-world).
	
9. Install on the local computer tool for deploying into the remote server (firebase-CLI). After that, we can execute Firebase's commands.
	
		> npm - g firebase-tools 

10. From commmand line (angular-hello-world folder) login into Firebase,

		> firebase login //to log into firebase account

11. Connect the app to the Firebase project to be deployed. We have to choose 'rewrite all: Y' (as we are cretaing a SPA app) and 
'index.html exists, owerwrite? N'

		> firebase init //connect the project in the folder we are in to the project in firebase. In the options, choose 'Hosting'.

12. Finally, deploy app into the remote server. We have to choose the dist folder (dist/angular-hello-world).

		> firebase deploy

When completed, firebase deploy command shows the information we need to visit (and to maintain) the app:<br>
Project Console: https://console.firebase.google.com/project/angular-hello-world-ab1fe/overview<br>
Hosting URL: https://angular-hello-world-ab1fe.web.app  //we can visit in this URL our work!


## 3.- Some examples of Angular+Bootstrap apps.

I expect to add some copy-paste examples in the future. For now, in the Examples folder, just an html file (the one I used before).
For now, instructions inside each file.<br>

<em>Last update of this repository: 2021-02-21 (repository creation)</em>