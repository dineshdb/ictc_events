# ictc events
Online web based ICTC events database.
..
## Getting started.
* Clone this repo.
* Update all submodules using ``` git submodule update --init --recursive```
* Build the backend.
* Create database 
* build frontend
* deploy frontend
* To sync new updates ``git pull --recurse-submodules``.

### Tools required
* Browsers and their developers tools
* Postman for managing and testing REST APIs
* node/npm, reactjs, etc

### Build Backend
* ``cd`` into backend
* Build using ``./gradlew build``
* Create required database and give permissions from [here](#create_database). If required, change configuration.
* Check the server using ``./gradlew bootRun``

#### Create Database
Install mysql or mariadb and get into its root shell. Then execute:
```mysql
mysql> create database dbms_project; -- Create the new database
mysql> create user 'dbms_project'@'localhost' identified by 'ThePassword'; -- Creates the user
mysql> grant all on dbms_project.* to 'dbms_project'@'localhost'; -- Gives all the privileges to the new user on the newly created database
```
**Note**: Don't forget to change password in production.

### Run Backend
* After building, there wil be a jar file in ``build/libs``.
* Run that jar file using ``java -jar ictc_events.jar``
* Check the api fron ``http://localhost:8080/``.

### Build Frontend
* ``cd`` into frontend.
* install all dependencies ``npm install``
* build the repo ``npm run build``.
* `use `npm run start` during development. It uses live reloading developement environment.
* collect the static artifacts and deploy into a static server using apache or nginx.


## Authors
* **[Rupesh Shrestha](https://github.com/RUPESH1439)** <rupesh.shrestha96742@gmail.com>
* **[Dinesh Bhattarai](https://dbhattarai.info.np)** <dbhattarai252@gmail.com>
* **[Jeevan Thapa](https://github.com/JeevanThapa9111)** <jeevanthapa911@gmail.com>
* **[Aashutosh Poudel](https://github.com/atosh502)** <aashutoshpoudyal@gmail.com>
