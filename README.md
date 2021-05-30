
# Udacity Blockchain Supply Chain

### UML Diagrams
  ![enter image description here](https://raw.githubusercontent.com/oluwaseye/udacity-blockchain-supply-chain/main/images/Udacity_Blockchain_Supply_Chain_1.png)
  ![enter image description here](https://raw.githubusercontent.com/oluwaseye/udacity-blockchain-supply-chain/main/images/Udacity_Blockchain_Supply_Chain_2__.png)
  ![enter image description here](https://raw.githubusercontent.com/oluwaseye/udacity-blockchain-supply-chain/main/images/Udacity_Blockchain_Supply_Chain_3.png)
  ### Libraries
  Below are the dependencies in my `packages.json` file:

     "dependencies": {
    	"truffle": "^5.1.51",
    	"truffle-assertions": "^0.9.2",
    	"truffle-hdwallet-provider": "^1.0.17",
    	"web3": "^1.3.0"
    }
**Why I used these libraries**:
-   `truffle`: truffle is a development framework for Ethereum that makes it easy to compile, test, and migrate solidity contracts to Ethereum networks.  I used  `truffle`  to deploy my smart contracts to the  `Rinkeby`  test network.
-   `truffle-assertions`: the library has convenience functions designed for solidity assertions inside of truffle tests.
-   `truffle-hdwallet-provider`: this libarary was used to enable my truffle deployments to spend test coins from my Metamask wallet on the Rinkeby network as part of deploying my contracts to  `Rinkeby`
-   `web3`:
-
### IPFS (InterPlanetary File System)
I did not use IPFS.

# Deployed to Ropsten Network*

**Transaction Hash**: 0xbbb837fa5274e7e6f722bb000a0cf1f2eef63b19ae5490b4cbc6227ebb3ef237

**Contract Address**: 0xe9906Eefe52Fed418C20c8B6b38cBDB60b1a9293

**Etherscan url**: https://ropsten.etherscan.io/tx/0xbbb837fa5274e7e6f722bb000a0cf1f2eef63b19ae5490b4cbc6227ebb3ef237

![enter image description here](https://raw.githubusercontent.com/oluwaseye/udacity-blockchain-supply-chain/main/images/deployment.png)
![enter image description here](https://raw.githubusercontent.com/oluwaseye/udacity-blockchain-supply-chain/main/images/deployment2.png)
![enter image description here](https://raw.githubusercontent.com/oluwaseye/udacity-blockchain-supply-chain/main/images/deployment3.png)
# Instructions
### Prerequisites

Please make sure you've already installed ganache-cli, Truffle and enabled MetaMask extension in your browser.

```
Give examples (to be clarified)

```

### [](https://github.com/galen211/udacity-blockchain-developer/blob/master/project3/INSTRUCTIONS.md#installing)Installing

A step by step series of examples that tell you have to get a development env running

Clone this repository:

```
git clone https://github.com/oluwaseye/udacity-blockchain-supply-chain

```

Change directory to  `coffee`  folder and install all requisite npm packages (as listed in  `package.json`):

```
cd coffee
npm install
```
Launch Ganache Desktop:

     Update the from value in ***truffle-config *rinkeby object***

In a separate terminal window, Compile smart contracts:

```
truffle compile
```
This will create the smart contract artifacts in folder `build\contracts`.
Migrate smart contracts to the locally running blockchain, ganache-cli:

```
truffle migrate
```
Test smart contracts:

```
truffle test

```
![enter image description here](https://raw.githubusercontent.com/oluwaseye/udacity-blockchain-supply-chain/main/images/test.png)
All 11 tests should pass.

 In a separate terminal window, launch the DApp:

```
npm run dev
```
![enter image description here](https://raw.githubusercontent.com/oluwaseye/udacity-blockchain-supply-chain/main/images/npmrundev.png)
