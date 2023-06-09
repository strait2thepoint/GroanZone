# Groan Zone
The Groan Zone is a website with a simple, blog-like layout. The content is intended to be all "dad jokes". The site is organized by jokes, which can each be upvoted or downvoted by visitors.

<hr>

![Node.js](https://img.shields.io/badge/Nodejs-16.18.0-blue.svg)
![Express.js](https://img.shields.io/badge/Express.js-4.17.1-blue.svg)
![Handlebars.js](https://img.shields.io/badge/Handlebars.js-4.7.7-blue.svg)
![Normalize.css](https://img.shields.io/badge/Normalize.css-8.0.1-blue.svg)

<hr>

# Description

1.   When visitors enter the Groan Zone, there is a login button that navigates to the login and signup pages for visitors. After login or signup, they are redirected to a page where they can create or add a new joke, allowing them to share their magical jokes.
2.  On the leftmost top corner, there is a "Go to all jokes" button that directs visitors to a splash page or a page that lists all jokes. This page displays the top five "dad jokes" of the day, providing visitors with a humorous outlet and a source of stress relief.
3.  Visitors have the option to register a user account or log in to their pre-existing account. Registered users can post jokes, which are then subject to upvoting and downvoting by other users.

Motivation :- The motivation behind this platform is to provide users with a dedicated space to share jokes, allowing people to find humor and take a break from everyday stress.


<hr>

## User Story

AS a developer, I want to have a website that displays jokes written by other users.

WHEN a user or a joke if added or removed in a local instance,

THEN that change is reflected in the globally hosted database.

WHEN a user impliments the delete feature,

THEN that user can add or delete jokes that they and only they have written.

WHEN I access the webpage on any different platform,

THEN the elements of the webpage are responsive and in compliance with formatting standards and best practices.

## Table of Contents

 *  [Installation](#installation)
 *  [Usage](#usage)
 *  [Assets](#Assets)
 *  [Testing](#testing)



## Installation
1. Install Node.js v16.
2. Intsall Mysql 8.0
3. Install inquirer, please use npm i inquirer@8.2.4
4. To connect with database, create file .env to store username, database name and password.
5. Run command npm install.
6. Navigate to db directory and run command "SOURCE schema.sql".
7. Tell MySQL to "USE joke_db;".
8. Navigate to seeds directory and run "node seeds/seed.js".
9. Now restart server by using command "npm start"

## Usage

The repository is available at:

https://github.com/strait2thepoint/DadJokeAPI

The link to the project is deployed at:

https://young-reef-43824.herokuapp.com/allJokes


## Assets:-


The following image demonstrates the website appearance:
1. Front Start login webpage
![Website](./assets/images/Front_login_page.png)

2. Web page which allow Login and signup.
![Website](./assets/images/login_signuppage.png)

3. Webpage will allow to create new joke webpage.
![Website](./assets/images/create_joke.png)

4. Webpage will displayed all jokes.
![Website](./assets/images/all_jokes.png)




## Testing

1. Stop server by using command "ctrl c"
2. Navigate to db directory and run command "SOURCE schema.sql";
3. Navigate to seeds directory and run "node seeds/seed.js";
4. Now restart server by using command "npm start"

### Test routes (append these after http://loclahost:3001):

/api/login              <-- POST only (log in a user)

/api/logout             <-- POST only (log out a user)

/api/users              <-- GET or POST (see a JSONified list of all users' data)

/api/users/:id          <-- GET         (see an individual user's data JSONified)

/api/jokes              <-- GET or POST    (see JSONified data for all jokes, or POST a new joke in JSON format)

/api/jokes/:id          <-- GET or DELETE  (see JSONified data for an individual joke, or DELETE an individual joke)

/api/jokes/upvote/:id   <-- PUT only       (alter the RATING data of an individual joke by incrementing it)

/api/jokes/downvote/:id <-- PUT only       (alter the RATING data of an individual joke by decrementing it)

## License

GNU General Public License v3.0 [![License: GPL v3](https://img.shields.io/badge/License-GPLv3-blue.svg)](https://www.gnu.org/licenses/gpl-3.0)


