## Please, note that this repositoty is under construction!

# Angular-Bootstrap!

Contents of this repo:

1.- How to create an Angular app.<br>
2.- How to deploy an Angular app into the server (to Firebase, in this case).<br>
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
Next command compiles our app and deployes it to the local server, port 4200. <br>
We can then in the browser run:
	
		> ng serve

5. View app in local browser (URL is showed by ng server when compile is finished) <br>
	
		> URL = http://localhost:4200/
	
6. Prepare the appp to be deployed to the remote server. Inside the app folder <br>

		> ng build --prod  // this creates a dist folder!
	
7. A new folder os created (folder = dist/angular-hello-world). That folder will be used to deploy to the remote server.


## 2.- How to deploy an Angular app into the server.

5. Deploy into a remote server. On my case, I choosed Firebase (free) hosting.
	
	After creating our account on Firebase we need to create a Project (with default settings).
	That is done in Firebase's Console. Pretty straitgt fordward. 
	The name could be (not needs to be) the same as the Angular (angular-hello-world).
	
	To be able of deploying. first, just once, we have to install firebase-cli 
	Again, with npm:
	
		> npm - g firebase-tools 


0. firebase login (to log into firebase account)
0b.- firebase init to connect the project in the folder we are in to the project in firebase WE Need to be in our angular project! choose hosting!

rewrite all: yes! we have a SPA (single page app)!
index.html exists, owerwrite? N!

Finally: firebase deploy  // that give us an URL !

Now, we have our local angular app connected to our project firebase. Lets deply it!
> firebase deploy

Project Console: https://console.firebase.google.com/project/angular-hello-world-ab1fe/overview
Hosting URL: https://angular-hello-world-ab1fe.web.app  // that's all


## 3.- Some examples of Angular+Bootstrap apps.

5. I expect to add some copy-paste examples in the future.


<em>Last update of this repository: 2021-02-20 (readme file reorganization) </em>