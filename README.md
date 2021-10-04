# URL-Shortener
I get quite easily annoyed by the length of URLs, and I got tired of having to see ads on websites to shorten a URL. So I decided to create a URL shortener of my own! This URL shortener is a Flask app that takes in a long URL and shortens it for the user. 

## Project Flow
The URL shortener takes in an input and the shortened URL is displayed on a new page after user input. This shortened URL successfully redirects the user to their originally inputted URL. For each long URL that is inputted by the user, this application randomly generates 3 alphabetic characters to be added to a shortened URL that redirects the user to their original inputted URL. 

To ensure that users do not have to put in URLs several times, I created a database and managed it using SQLAlchemy as an Object Relational Mapper (ORM) Tool to convert function calls to SQL statements. This means that if users were to input the same link twice, the application will return the same shortened link to ensure that the shortened URL returns the user to the same original longer URL.

## Git Clone

To clone this repository, run the following line in your command line or Terminal. 

`git clone https://github.com/reeteshsudhakar/URL-shortener`

Once the code is run, a locally hosted web app will open to the home page of the shortener, prompting the user to enter a URL to be shortened! 

## To-Do List
* [ ] Exceptions and Error Handling - errors, warnings, etc. 
* [ ] Heroku Website Hosting
* [ ] Website Design and Aesthetics 
* [ ] Check database management
