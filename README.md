# Decentralized Star Notary by Satyadeep

## Getting Started

These instructions will get you a copy of the project up and running on your local machine for development and testing purposes.

### Prerequisites
- [npm](https://www.npmjs.com/) (Node.js package manager)
- [Truffle](https://truffleframework.com/) to compile, deploy and test smart contracts.
- [OpenZeppelin](https://openzeppelin.org/) to make ERC-721 tokens easily.
- [http-server](https://www.npmjs.com/package/http-server) A command-line http server.
- [Metamask](https://metamask.io/) Ether wallet.

### Install necessary packages

- Install http-server if you don't have it yet.
```
npm install http-server -g
```

- Install Truffle if you don't have it yet.
```
npm install truffle -g
```

- Install Truffle HDWallet Provider
```
npm install --save truffle-hdwallet-provider
```

### Configuring

- Initialize Truffle
```
truffle init
```

- Go to [Infura.io](https://www.infura.io/). 
  - Create an account and a new project.
  - Change the endpoint to **Rinkeby** Test Network.
  - Copy the link to be used later in the truffle.js configuration part.

- Install Metamask and create account.
  - Make sure to point to **Rinkeby** network.
  - To fund your wallet to be used for **Rinkeby** network, go to this (faucet)[https://faucet.rinkeby.io/] and follow the instructions.
  - Get the wallet seed to be used later in the the truffle.js configuration part.

- Create file **.mnemonic** with the Metamask seed you got from above instructions.
- Create file **.infura-key** with the Infura link you got from above instructions.

### start server
npm run dev

### Testing, Compile, Deploy smart contracts using Truffle

- Enter Truffle development environment
```
truffle develop
```

- To run unit tests
```
truffle(develop)> test
```

- To compile smart contract
```
truffle(develop)> compile
```

- To migrate for the first time to **Rinkeby** Test Network
```
truffle(develop)> migrate --network Rinkeby
```
or 
- To migrate onwards
```
truffle(develop)> migrate --reset --network Rinkeby
```

- To migrate for the first time to local blockchain
```
truffle(develop)> migrate
```
or 
- To migrate onwards
```
truffle(develop)> migrate --reset
```


## Versions

* Truffle v5.0.19
* openzeppelin-solidity": v2.3.0
* "truffle-hdwallet-provider": v1.0.9

	## Token details

* ERC-721 Token Name: Star Notary Token
* ERC-721 Token Symbol: SNT
* Token Address on the Rinkeby Network: [0x5D8f3B449C1602a08d478A4a994964590CB6dbda](https://rinkeby.etherscan.io/address/0x5D8f3B449C1602a08d478A4a994964590CB6dbda)

Code Source Help & Reference: Internet Websites & https://github.com/thom/udacity-blockchain-developer-nanodegree/tree/master/project-5

