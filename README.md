# Crowd Funding


## Build

### Prerequisites
Metamask,Truffle and ganache have to be installed

```shell
npm install -g truffle
```

After installation, open Ganache and start a workspace. Ensure the host and port in `truffle-config.js` is the same as the port in that workspace.

```javascript
// truffle-config.js
development: {
	host: "127.0.0.1",
	port: 7545,
	network_id: "*",
}
```

compiling the samrt contract 

```shell
truffle compile
```

deploying the smart contract.

```shell
truffle migrate
```

After that, replace the address in `src/eth/CrowdFunding.js`  with the address of CrowdFunding contract in Ganache.

```javascript
// CrowdFunding.js
const address = '0xA305BC95CBf8E6D4d540466C39C02DF3b2744031';
```


install all dependencies necessary

```shell
yarn install
```

## Run

Start frontend application 

```shell
yarn start
```

