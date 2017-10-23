# Saturday-10-7-2017
SMU Class Saturday 10-7-2017

DISCUSSED REVISION FROM LAST CLASS

INSTALLED HOMEBREW
INSTALLED MYSQL
INSTALLED MYSQL-WORKBENCH
ruby -e "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/master/install)"



started server on MySQL with mysqld &
the & to run in the background

created db
created table

exercise
 anmiaml.db
 favorite.db

 Instructions

Now it is your turn to set up a localhost connection! This may seem as if it will be an easy task, but there are some common errors and hurdles that might stand in your way as you work to create your first ever MySQL connection.

Start out by opening up MySQL Workbench and hitting the (+) button next to the text which reads "MySQL Connections". Sequel Pro will also have a (+) on the bottom left for new connections.

Enter the following credentials into the on-screen prompt...

Connection Name: Local Instance MySQL

Connection Method: Standard (TCP/IP)

Hostname: localhost

Port: 3306

Username: <Your MySQL Username> (Defaults to "root")

Password: <Your MySQL Password> (Defaults to empty)

Keep the Default Schema field empty

Hit "Test Connection" and, if the connection is successful, hit okay and double-click on the newly created field under the "MySQL Connections" text on the home page

If the connection fails, raise your hand and one of us will come around to help you out. Until we come by, however, take this time to go online and see if there is anything online which might tell you what went wrong. Do not worry if you cannot find anything though, we will make sure to figure this out.
If your connection was successful and you have nothing else to do, feel free to help those around you in creating their connections.

BONUS: Look into how you can create and use databases using SQL commands

BONUS: Look into the reasons why MySQL uses port 3306 as its default

XXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXX
favorites;

Instructions

It is time to add some data into FavoriteDB! The data that you add should be unique to you and you should try to test your skills in not only adding new data, but also attempt to update old data as well!

Try to add at least three rows of data to each table.

BONUS: Look into how you you might go about creating a column that can hold a default value within it and how default values work when creating new rows.

BONUS: Look into how you might go about creating a column with a default value that automatically go up with each new row

BONUS: Look into the concept of making a column the "primary key"

ULTRA BONUS: Try to create a column called "id" in one of your tables that can contain an integer, is the primary key for the table, cannot be NULL, and automatically increments with each new row added.

Oct 7, Scratch

MySQL WorkBench Launch

*** BE PROACTIVE IN SEEKING TA/INSTR HELP ON SETTING UP ***

Databases:

Persistence: KEEP ON / STAY / CONTINUE /NOT GOING AWAY

Server Side persistent data:
- With node:
 - saved modules locally on our server - FILES
 - Bank.js - Text files : module used => "fs"

 WHY NOT JUST USE FILES:
 - NOT VERY ORGANIZED
 - LIMITED IN THE WAYS WE CAN INTERACT with DATA

 Another database: Firebase

 What structure of data? format?
 - JSON objects
 - KEY/VALUE PAIRS
 - hierarchical struc.


BLOG:

- articles (title, body, keywords, date, author, category/topic, comments, multimedia, suggestions),
- authors (name, contact info, affiliation, bio, multimedia)
- comments (text, commenter, ratings, datetime)
- keywords
- categories

create database blog;

create table articles (
    id integer(11) auto_increment not null primary key,
    title varchar(256) not null,
    body text,
    date datetime,
    author_id integer(11)

);

create table authors (
 id integer(11) auto_increment not null primary key,
 name varchar(1000),
 contact_email varchar(1000),
 affiliation varchar(256),
 bio text
);












article = {
    title: jhjhj,
    author: {
        name: jshj,
        contact_info: bbb
    }

}

Relational Databases = TABLE based
EXCEL spreadsheets

TABLES for BLOG:

1. articles
2. authors
3. comments
==============================
SQL  = Structured Query Language

MySQL =
===============================

FREE OPEN SOURCE vs PAID Relational DBs

- MySQL, PostgreSQL, SQLlite (simplest)

PAID ONEs:
- Oracle
- MsSQL / SQL Server

- MySQL WorkBench

=================== Database Servers ============
Server = who provides service
= available all the time
= provides specific service
= available at WELL KNOWN location

DB servers:
- provide read, write access to persistent data
- also provide mapping/formatting/ finding data

MySQL:
- Well known locations in computers == PORTS
- 80 = http, 443 = https, ssh = 22

- MySQL = 3306 (well known and common)

Local = on our machines = MYSQL Server/Daemon

Need to start a MySQL server
Need to use a MySQL client

MySQLWOrkBench == Our client
Client == helps us do stuff with the server easily

IF FORGOTTEN ROOT PASSWORD =>
 completely uninstall EVERYTHING related to MySQL
REINSTALL


MySQL is CASE INDEPENDENT;

cape === CAPE

INSERT === insert

name vs Name = all the same;
