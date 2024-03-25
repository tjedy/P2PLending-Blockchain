# HYPERLEDGER FABRIC SYSTEM MONITORING WEB APPLICATION

This web explorer application is intended to help monitor transactions and blocks occurring on the deployed Hyperledger Fabric network.
This web explorer application is forked from [Hyperledger Explorer](https://github.com/hyperledger/blockchain-explorer/tree/release-3.2) and adjusted to suit the system's business processes.

## General introduction

### Group of authors

1453044 - Nguyen Hoang Thien
1453045 - Nguyen Chau Thanh Thien

### Instructor

Dr. Dinh Ba Tien - Head of IT Department, University of Natural Sciences
Nguyen Thanh Son - Head of PayooX, VietUnion

## System introduction

### Library used

* [Node.js](https://nodejs.org/en/) - Back-end building platform
* [Express.js](https://expressjs.com/) - Library to support building server APIs
* [PostgreSQL](https://www.postgresql.org/) - PostgreSQL relational database
* [ReactJS](https://reactjs.org/) - Platform for building web interfaces

### Basic functions

* Dashboard - View overview information of the current network (Block number, transactions, nodes, chaincode, timeline)
* Block - View overview information of a data block
* Transaction - View detailed information of a transaction
* User view (open with mobile app) - View transaction details that that user created

## Deployment

### Request

* Install Node.js version 8.10.0 or higher
* Install npm version 5.x or higher
* Install PosrgreSQL version 10
* Install Heroku version 7.0.26 or later
* Install git 2.9.x or higher

### Instructions run on localhost platform

1. Run the PostgreSQL server on port 5432
2. Adjust the appconfig.json file to suit the deployed blockchain network. If you reuse the system deployed by the team, skip this step
3. In the app/db directory, run the psql command and execute two files explorerpg.sql and update.sql to create data storage tables
4. In the client directory, run the npm run build command
5. In the root directory, run npm install command
6. Access the link https://localhost:8080

### Instructions to run on heroku environment

1. Login to heroku - heroku login
2. Run the heroku create command
3. Install Postgres heroku addon on heroku web
4. Run command psql and execute 2 files explorerpg.sql and update.sql for the newly created database addon
4. Run the command git add .
5. Run the command git commit -am "Deploy Hyperledger Explorer"
6. Run the command git push heroku master
7. Heroku announces deployment status
(Implemented group Endpoint API: https://aqueous-hollows-61580.herokuapp.com/)

## License

This system is owned by the author group, protected by intellectual property rights according to the regulations of the University of Natural Sciences and Online Services Joint Stock Company (VietUnion).