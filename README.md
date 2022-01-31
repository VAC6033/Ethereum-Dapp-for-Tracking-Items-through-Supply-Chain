Ethereum DApp for Tracking Items through Supply Chain

Versions used:

Truffle v5.4.0 (core: 5.4.0)
TRUFFLE OVERVIEW
A world class development environment, testing framework and asset pipeline for blockchains using the Ethereum Virtual Machine (EVM), aiming to make life as a developer easier. With Truffle, you get:

Built-in smart contract compilation, linking, deployment and binary management.
Automated contract testing for rapid development.
Scriptable, extensible deployment & migrations framework.
Network management for deploying to any number of public & private networks.
Package management with EthPM & NPM, using the ERC190 standard.
Interactive console for direct contract communication.
Configurable build pipeline with support for tight integration.
External script runner that executes scripts within a Truffle environment.
Web3.js - 1.3.4
The web3.js library is a collection of modules that contain functionality for the ethereum ecosystem.

Simply, it provides us with an API to use so we can easily work with the blockchain. Web3 works as a wrapper for JSON RPC to connect to a remote or local Ethereum node with either a HTTP or IPC connection. Web3 is basically a connection between the Ethereum blockchain and your smart contract.

Solidity - 0.8.3 (solc-js)
Solidity is an object-oriented programming language for writing smart contracts. It is used for implementing smart contracts on Ethereum and other platforms.

Getting Started

Clone this repository.
Install the dependencies with NodeJS and NPM.
Test the application making calls to the contract on the Rinkeby Test Network.
Take a look at the transactions happening on the Rinkeby Test Network at Etherscan explorer.
Important: You will need your personal passphrase from your Ethereum account to publish into the Rinkeby Test Network, hence the .secret file in the truffle-config.js, even tough being a test network.

Instructions

Install the dependencies:
  npm i
Turn on the Ganache suite so that you will have pre-defined accounts to test the contracts:

Migrate, compile and test the contracts with truffle (on a separate console). It will use the previously up and running ganache locally blockchain.

  truffle migrate
  truffle compile
  truffle test
state

Publish the contracts into the Rinkeby Test Network with your Infura key:
  truffle migrate --reset --network rinkeby
Check out and test the DApp in the frontend with the command below. You can run on the ganache-cli window, since Ganache was only for testing purpose.
  npm run dev
