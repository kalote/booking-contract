# booking-contract

Booking backend system using solidity contract to provide the following feature:

- Get room per id (using public visibility on `rooms` mapping)
- Book a room
- Cancel a booking

# Local install

This project is based on truffle. In order to run, here is my recommendation (other approach are possible though ...):

- Install [Ganache](https://www.trufflesuite.com/ganache) (the delicious UI that creates a local blockchain)
- Launch Ganache and create a new workspace using default settings (ethereum based / port 7545)
- Run `npm install` to install dep
- Run `npm run migrate` to deploy the contract on the Ganache testing chain

_If you have any issue, check `truflle-config.js` and update according to your setup_

When deployed, run `npm run test` to check if everything is working as expected.

Finally, retrieve the contract address and use it in the [booking-frontend](https://github.com/kalote/booking-frontend/)

You will need to configure MetaMask to connect to your local blockchain. The settings for using Ganache on MetaMask are the following:

- Name: ganache
- RPC URL: http://localhost:7545
- ChainID: 1337
- Currency symbol: ETH
