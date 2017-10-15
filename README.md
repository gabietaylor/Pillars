# Pillars - Restructuring Humanity




This document outlines the base requirements for Project 2.

Requirements

Your project must:

Use a Node and Express Web Server;

Be backed by a MySQL Database an ORM (not necessarily Sequelize);

Have both GET and POST routes for retrieving and adding new data;

Be deployed using Heroku (with Data);

Utilize at least one NEW library, a MINIMUM of 3 new NPM packages, or technologies that we haven’t discussed;

Have a polished frontend / UI;

Have folder structure that meets MVC Paradigm;

Meet good quality coding standards (indentation, scoping, naming).

Suggestions

Your project should:

Incorporate Basic Testing Framework, see Project Suggestions;
# Pillars - Restructuring Humanity

![lucidchart1](https://github.com/cphelps987/Project2/blob/master/lucidchart.png)

# Pseudo Code

# MVP (Minimum Viable Product)
* **A chat that is anonymous and deletes + have helpful resources**
* **Make sure it fixes a problem**

## DATABASE INFO

## CHATROOM TABLE
* ID (primary key)
* link (url)
* title
* moderators 
* moderation level
* password

## USER TABLE
* ID (primary key)
* UserName
* Password
* role (user, admin, mod)
* verifiedUser
* userScore (based on up votes)
* flagged

## HELPFUL RESOURCES TABLE
* ID (primary key)
* title
* facebook
* twitter
* description
* link
* userScore (based on up votes)

## FAQ TABLE
* ID (primary key)
* question
* answer

## NOTSONICE TABLE
* **words to filter through**
* ID (primary key)
* wordlist 
* category: racist, offensive, sexist


### NPMS:
* socket io
* passport/oauth (we still need google for authentication) || (https://www.npmjs.com/package/simple-oauth2, https://oauth.net/2/)
* geolocation (future?)
* chalk(?)
* emoji(?)
* regexp(to filter offensive words)

### Project Outline
* Get all of the npm packages and require them in server.js
* Create databases
* **Break up server files by npm package**
* Make a markup of the frontend
* Make sure all of the packages/dbs work with the frontend
* Make sure we can set up multiple chats at one time
* Figure out how to push passport data into database
* **NEW LIBRARY - browser notifications**
* **Make sure chat deletes (orm)** 
* **No cookies**
* **Dont HAVE to login**
* **Search bar to search for chats**
* **private** chats
* Look at google recaptcha (https://www.google.com/recaptcha/intro/)

### ORM PSEUDOCODE
* passport
* username
* password
* link database for helpful resources
* if "admin" > show EVERYTHING, if "user" > show links, chat titles.

### Disclaimers:
* If this is a serious medical issue, please call 911
* No one here is a professional psychiatrist.......

### Stuff we need to talk about:
* Do we need a separate database for the chat or can we rely on socket io?
* Does socket io have a delete function?


### Future Developments:
* Real-Time Help
* Local chat rooms
* If the person was helpful
* Causes (Meetup for aids, cancer, etc)
* Gives you default icon options
* Add password reset and send user email
* Prevent bots by making sure you cant say the same thing twice

### Presentation
* Video of it working
* Send link out to class channel and have people test it?

## STATUS ON JULY 12

## Working
* chat (working seperately)
* passport
* handlebars rendering (talking to server)

## Need
* Put data into databases
* Create dummy users 
* **CONTENT**
* Add disclaimers and about us/contact page
* Make it look pretty
* **Add socket io chat to page**
* socket io last resort (redirect to chat page)
* call orm in connection js inside if statements!

## STATUS ON JULY 13

* **GABIE AND SAKINA: NEW CHAT**
* COURTNEY: Getting orm from backend to front (on page) & heroku(?)
* MARC: Finish making all the pages and make them look nice 
* MEL: Help marc with front end
* JASMINE AND NIGHTMARE!!!!! :weary:

# Project Guidelines
This document outlines the base requirements for Project 2.

Requirements

Your project must:

Use a Node and Express Web Server;

Be backed by a MySQL Database an ORM (not necessarily Sequelize);

Have both GET and POST routes for retrieving and adding new data;

Be deployed using Heroku (with Data);

Utilize at least one NEW library, a MINIMUM of 3 new NPM packages, or technologies that we haven’t discussed;

Have a polished frontend / UI;

Have folder structure that meets MVC Paradigm;

Meet good quality coding standards (indentation, scoping, naming).

Suggestions

Your project should:

Incorporate Basic Testing Framework, see Project Suggestions;

Use Handlebars for Server-Side Templating

Incorporate Authentication (JSON Web Tokens, Sessions, Etc.)

Create a migration strategy for sharing data across team members.

Use Handlebars for Server-Side Templating

Incorporate Authentication (JSON Web Tokens, Sessions, Etc.)

Create a migration strategy for sharing data across team members.
