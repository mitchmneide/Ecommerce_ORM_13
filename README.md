# E-commerce Back End Starter Code
![Github license](https://img.shields.io/badge/license-MIT-blue.svg)

## Description
Backend for E-Commerce site through use of command line with API testing in Insomnia. 
Walkthrough Video: 

## Table of Contents
- [Installation](#installation)
- [Usage](#usage)


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
If error occurs do be sure you deleted the .EXAMPLE on .env provided
Once that is done you are reading to go! Start up the server with `Node server` or `npm start` And be sure to have the Insomnia app ready to go!

This project has 3 endpoints `/categories/` `/tags/` `/products/`

Within each of these you can test the following routes GET/POST/PUT/DELETE

GET you can access all of the data in the database or after the / you can input the id of data and GET the selected one.
POST you can add a new category/tag/product with the correct 
