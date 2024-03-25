# SMART CONTRACT STRUCTURE FOR P2P-LENDING NETWORK

Smart Contract stores information about contracts arising during the loan process, stored on the blockchain under the consensus of ledgers in the network.

## General introduction

### Group of authors

1453044 - Nguyen Hoang Thien
1453045 - Nguyen Chau Thanh Thien

### Instructor

Dr. Dinh Ba Tien - Head of IT Department, University of Natural Sciences
Nguyen Thanh Son - Head of PayooX, VietUnion

## System introduction

### Tools used

* [Visual Studio Code](https://code.visualstudio.com/) - IDE that supports programming
* [Hyperledger Composer Add-on](https://github.com/hyperledger/composer-vscode-plugin) - plugin on VSC that supports model structure, logic, permissions for the Fabric system
* [Hyperledger Composer Playground](http://composer-playground.mybluemix.net/) - supports testing the structure of programmed smart contracts
* [Hyperledger Composer CLI](https://github.com/hyperledger/composer) - supports installing, testing, deploying, and monitoring blockchain systems using the command line
* [Hyperledger Composer Node.js SDK](https://github.com/hyperledger/composer) - Library to support building with Hyperledger Fabric system with Composer

### Structure of basic Contracts

* LoanContract - Stores loan and related borrower information
* InvestingContract - Stores loan investment commitment information and related investors
* SettlementContract - Stores a payment term of the loan, made by the borrower
* InvestingFeeContract - Stores information about the platform's service fees corresponding to a payment term of a set of investment commitments.

## Network deployment

### Request

* Install Node.js version 8.10.0 or higher
* Install npm version 5.x or higher
* Install [Hyperledger Fabric](https://hyperledger-fabric.readthedocs.io/en/release-1.0/getting_started.html)
* Install [Hyperledger Composer](https://hyperledger.github.io/composer/latest/installing/development-tools.html)


### Instructions for deploying network at localhost

* Follow the instructions of [Hyperledger Composer](https://hyperledger.github.io/composer/latest/tutorials/deploy-to-fabric-single-org)

### Instructions for deploying a network at IBM Kubernetes IBM Service

1. Follow the instructions [IBM Container Service](ibm-container-service.md)
2. Open the link https://your-kubernetes-public-ip:31080 or http://173.193.120.168:31080 (prepared by the team)
3. Create a new business network archive with user = admin and password = password (Deploy new business network button)
4. Open the newly created BNA.
5. Upload the files model.cto, permission.acl, logic.js and execute the update command
(Note: If you use the IP created by the group, please do not change existing BNAs because it affects the current system. If you cannot access the IP, contact the group to re-issue a new IP due to Kuberbetes policy. will change cluster once a month)

## License

This system is owned by the author group, protected by intellectual property rights according to the regulations of the University of Natural Sciences and Online Services Joint Stock Company (VietUnion).
