> [!CAUTION]
> **ARCHIVED LEGACY WEB WALLET — DO NOT USE WITH QWERTYCOIN V2.**
> This application is unsupported and incompatible with the current wallet,
> network, and restricted-RPC architecture. Do not enter a seed or private key
> and do not receive or send funds with it. Use the current
> [Web Wallet](https://wallet.qwertycoin.org/) from its
> [maintained source](https://github.com/qwertycoin-org/wallet.qwertycoin.org).

![image](https://cdn.qwertycoin.org/images/press/other/qwc-github-3.png)
#### Master Build Status
[![Build Status](https://travis-ci.org/qwertycoin-org/webwallet-js.svg?branch=master)](https://travis-ci.org/qwertycoin-org/webwallet-js) [![Build status](https://ci.appveyor.com/api/projects/status/rvsgv9p8wbolxfkt/branch/master?svg=true)](https://ci.appveyor.com/project/Qwertycoin/webwallet-js-iiaw6/branch/master)

# Qwertycoin Web Wallet - Fully client-side
This web wallet is doing everything client-side to give the best privacy to users.
The API servers are currently only used to optimize the communication with the daemon and compress the blockchain.

# Security
**No keys, seeds, or sensitive data is sent to the server**  
If you find a potential security issue, please contact me so we/I can patch it as soon as possible.  
Encryption is done with a certified library, [Tweetnacl.Js.](https://github.com/dchest/tweetnacl-js)

# Features (non-exhaustive)
- Complete wallet sync without server side processing for security
- Receive/send history
- Mempool support to check incoming transfers
- Send coins - including QR code scanning and subaddress support
- Receive page to generate a custom QR code
- Import from private keys, mnemonic seed, or json file (exported by the wallet)
- Export private keys, mnemonic phrase, or json file (which include all the history)
- View only wallet
- Basic network stats

# How to compile & Deploy
The project is using Typescript as main language everything else (dependencies) is already included.

## Compilation
The first step will be to compile the typescript code into javascript code so browsers will be able to understand it. 
You also need to build some files that are dynamically generated like the manifest ...
This task is doable with :
```
npm install
nodejs ./node_modules/typescript/bin/tsc --project tsconfig.json
nodejs build.js
```
The first task install dependencies (typescript) and the text one compile the typescript code.
We are using a custom tsconfig file which is optimized for production.

## Deploy
All the content of the src directory needs to be exposed with a web-server.

## Change configuration
You will have to edit the file src/config.ts in order to change the API endpoint. 

That's all

### Donate

```
QWC: QWC1K6XEhCC1WsZzT9RRVpc1MLXXdHVKt2BUGSrsmkkXAvqh52sVnNc1pYmoF2TEXsAvZnyPaZu8MW3S8EWHNfAh7X2xa63P7Y
```
```
BTC: 1DkocMNiqFkbjhCmG4sg9zYQbi4YuguFWw
```
```
ETH: 0xA660Fb28C06542258bd740973c17F2632dff2517
```
```
BCH: qz975ndvcechzywtz59xpkt2hhdzkzt3vvt8762yk9
```
```
XMR: 47gmN4GMQ17Veur5YEpru7eCQc5A65DaWUThZa9z9bP6jNMYXPKAyjDcAW4RzNYbRChEwnKu1H3qt9FPW9CnpwZgNscKawX
```
```
ETN: etnkJXJFqiH9FCt6Gq2HWHPeY92YFsmvKX7qaysvnV11M796Xmovo2nSu6EUCMnniqRqAhKX9AQp31GbG3M2DiVM3qRDSQ5Vwq
```

### Contributors and thanks

#### Developers:
- gnock (main)
- cryptochangements
- davehlong (initial adaptation of PHP Api for Bytecoin based coins)
- aiwe (adapted for Bytecoin/CryptoNote from Monero codebase)
- nnian, ExploShot (adapted for Qwertycoin codebase)

#### Translations:
- Chinese: mainframer, [Alex Nnian - Qwertycoin](https://github.com/qwertycoin-org)
- English: too many people
- French: gnock
- German: F0sching, [Alex Nnian - Qwertycoin](https://github.com/qwertycoin-org)
- Greek: GeraltOfTrivia
- Hungarian: Gelesztaa
- Italian: unknown :(
- Japanese: [Alex Nnian - Qwertycoin](https://github.com/qwertycoin-org)
- Korean: [Xecute0101 - Qwertycoin](https://github.com/qwertycoin-org)
- Persian: M4hdi1995
- Russian: [Aiwe](https://github.com/aivve)
- Serbian cyrillic: girugameshh
- Spanish: [Guerreru](https://github.com/Guerreru)
- Ukrainian: [Aiwe](https://github.com/aivve)

#### Incomplete Translations:
- [Arabic](https://github.com/qwertycoin-org/webwallet-js/blob/master/src/translations/ar.json)
- [Hebrew](https://github.com/qwertycoin-org/webwallet-js/blob/master/src/translations/he.json)
- [Hindi](https://github.com/qwertycoin-org/webwallet-js/blob/master/src/translations/hi.json)
- [Polish](https://github.com/qwertycoin-org/webwallet-js/blob/master/src/translations/pl.json)
- [Portuguese](https://github.com/qwertycoin-org/webwallet-js/blob/master/src/translations/pk.json)
- [Romanian](https://github.com/qwertycoin-org/webwallet-js/blob/master/src/translations/ro.json)
- [Turkish](https://github.com/qwertycoin-org/webwallet-js/blob/master/src/translations/tr.json)
- [Urdu](https://github.com/qwertycoin-org/webwallet-js/blob/master/src/translations/pk.json)
- [Vietnamese ](https://github.com/qwertycoin-org/webwallet-js/blob/master/src/translations/vn.json)
