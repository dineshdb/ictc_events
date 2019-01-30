# ictc events
Online web based ICTC events database.

### Tools required
* Browsers and their developers tools
* Postman for managing and testing REST APIs
* node/npm, reactjs, etc

## Getting started for development
* Clone this repo.
* Update all submodules using ``` git submodule update --init --recursive```
* Update each submodule individually (since submodules can get out of sync in development).
* Create database 
* run backend
* run frontend and proxy

### Create Database
Install mysql or mariadb and get into its root shell. Then execute:
```mysql
mysql> create database dbms_project; -- Create the new database
mysql> create user 'dbms_project'@'localhost' identified by 'ThePassword'; -- Creates the user
mysql> grant all on dbms_project.* to 'dbms_project'@'localhost'; -- Gives all the privileges to the new user on the newly created database
```

### Build and run backend
Make sure you have setup database as described above.
* ``cd`` into backend
* Build using ``./gradlew build``
* Check the server using ``./gradlew bootRun``

### Build and run frontend
* ``cd`` into frontend.
* install all dependencies ``npm install``
* `use `npm run live` during development. It uses live reloading developement environment.

## Getting started for production
[TODO]

## Authors
* **[Rupesh Shrestha](https://github.com/RUPESH1439)** <rupesh.shrestha96742@gmail.com>
* **[Dinesh Bhattarai](https://dbhattarai.info.np)** <dbhattarai252@gmail.com>
* **[Jeevan Thapa](https://github.com/JeevanThapa9111)** <jeevanthapa911@gmail.com>
* **[Aashutosh Poudel](https://github.com/atosh502)** <aashutoshpoudyal@gmail.com>
