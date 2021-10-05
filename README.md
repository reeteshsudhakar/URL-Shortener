# URL-Shortener
I get quite easily annoyed by the length of URLs, and I got tired of having to see ads on websites to shorten a URL. So I decided to create a URL shortener of my own! This URL shortener is a Flask app that takes in a long URL and shortens it for the user. 

## Project Flow
The URL shortener takes in an input and the shortened URL is displayed on a new page after user input. This shortened URL successfully redirects the user to their originally inputted URL. For each long URL that is inputted by the user, this application randomly generates 3 alphabetic characters to be added to a shortened URL that redirects the user to their original inputted URL. 

To ensure that users do not have to put in URLs several times, I created a database and managed it using SQLAlchemy as an Object Relational Mapper (ORM) Tool to convert function calls to SQL statements. This means that if users were to input the same link twice, the application will return the same shortened link to ensure that the shortened URL returns the user to the same original longer URL.

## Web Deployment
Using the Heroku CLI, this Flask app was successfully deployed to [this website](https://shorten-your-url.herokuapp.com/). To deploy the web app using Heroku, this repository was first created. Next, a requirements file and Procfile were created and added to the repository. After these were created, the following lines were run in the command line or Terminal.

Logging into Heroku using credentials:

`heroku login -i`

Adding the repository to the remote one:

`heroku git:remote -a {URL-shortener}`
> **Note**: If you want to deploy a web app using Heroku, you would pass in the name of your desired repository that stores the source code in the curly brackets.

Uploading the project by pushing it to Heroku:

`git push heroku master`

After these commands were run, a progress log will show up in the command line or Terminal, and the app will be successfully deployed to Heroku. 

## Git Clone

To clone this repository, run the following line in your command line or Terminal.

`git clone https://github.com/reeteshsudhakar/URL-shortener`

Once the code is run, a locally hosted web app will open to the home page of the shortener, prompting the user to enter a URL to be shortened! 

## To-Do List
* [ ] Exceptions and Error Handling - errors, warnings, etc. 
* [X] Heroku Website Hosting
* [ ] Website Design and Aesthetics 
* [X] Check database management
