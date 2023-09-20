# Crypto Media Network Coin Studio



![Crypto Media Network Coin Studio architecture](../../.gitbook/assets/image%20%283%29.png)

## Backend Infrastructure

The backend is composed of the following independent services

* Studio API Backend has two purposes. Provides an API for fast and convenient querying of the blockchain data for the Studio DApp. Transmits heavy and complicated transaction flows on behalf of the user.
* Crypto Media Network Coin-funder service used to fund community members and wallet users on the Crypto Media Network Coin blockchain.
* Crypto Media Network Coin IPFS proxy used for fast fetching and storing data in IPFS.

## Contracts

Crypto Media Network Coin studio is designed to launch DeFi communities on the Crypto Media Network Coin network. The community contract binds together most of the services and features of the Studio. Among other things it consists of:

* Entities List contract to store community members and their roles
* Community Crypto Media Network20 tokens on Crypto Media Network Coin network with transfer rules
* Crypto Media Network20 tokens on Ethereum. This is the token that the user issues as part of the community deployment process
* [Multitoken bridge](https://github.com/Crypto Media Networkio/bridge-contracts) - to minimize friction and costs we extended the POA Crypto Media Network20-Crypto Media Network20 bridge contract to many-Crypto Media Network20-to-many contract.

## Plugins

The plugins are used to customize the community to your specific needs. These can be smart contracts, backend services or the integration of both. The currently available plugins are:

* Business List - allows you to add businesses to you community. Businesses are Entities List members with special roles.
* Join Bonus - define a join bonus for new community members.
* Fiat Ramp - Currently integrated to [Transak](https://transak.com/) and [Moonpay](https://www.moonpay.io/) to allow easy deposit and withdraw using Bank Accounts and Payment Cards.
* More plug-ins coming soon.

