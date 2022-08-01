# E-commerce Back End Starter Code
![Github license](https://img.shields.io/badge/license-MIT-blue.svg)

## Description
Backend for E-Commerce site through use of command line with API testing in Insomnia. 
Walkthrough Video: [Click Here](https://drive.google.com/file/d/1bZ3MPLNy-qdryVFdI7hCV5cVOdTED9Pf/view?usp=sharing)

## Table of Contents
- [Installation](#installation)
- [Usage](#usage)
- [Libraries](#libraries)
- [License](#license)
- [Credits](#credits)
## Installation 
To use this project, the user must have Node.js and MySQL installed.  
This project use dotenv, Express, MySQL2 and Sequelize. To initialize these use `npm init -y` then use `npm install` or `npm i` for short.

## Usage 
In order for you to use the schema in the MySQL shell you must use the following commands. Provided an .env.Example in order to use properly please delete example and enter your required information for MySQL
```
mysql -u <root/the username under your mysql command> -p
you'll be prompted for the password
mysql> source db/schema.sql
```
You can follow that up with quit to exit out of the MySQL shell
Next you'll need get the seed data in the command line type `npm run seed`
If error occurs do be sure you deleted the .EXAMPLE on .env provided</br>
Once that is done you are ready to go! Start up the server with `Node server` or `npm start` And be sure to have the Insomnia app ready to go!

This project has 3 endpoints `/categories/` `/tags/` `/products/`

Within each of these you can test the following routes GET/POST/PUT/DELETE

GET you can access all of the data in the database or after the / you can input the id of data and GET the selected one.
POST you can add a new category/tag/product with the correct syntax of course
Products 
```
{
    "product_name": "Swim Shorts",
	"price": 15,
	"stock": 20,
	"category_id": 2,
	"tagIds": [3,4,5,6]
}
```
Tags
```
{
    "tag_name": "yellow"
}
```

Categories 
```
{
	"category_name": "Video Games"
}
```

As for PUT you can update data from selected ID numbers follwing the syntax from above in their selective routes
And DELETE will destroy the data with ID provided

## Libraries 
- [dotenv](https://www.npmjs.com/package/dotenv)
- [Express.js](https://expressjs.com/)
- [Sequelize](https://www.npmjs.com/package/sequelize)
- [MySQL2](https://www.npmjs.com/package/mysql2)
- [Node.js](https://nodejs.dev/)

## License
&copy; 2022 by Mitchel Eide

This project is licensed under the MIT License
[License: MIT License](https://opensource.org/licenses/MIT)

## Credits 
Stater code cloned from [Xandromus](https://github.com/coding-boot-camp/fantastic-umbrella) 