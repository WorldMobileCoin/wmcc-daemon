
# wmcc-daemon (WorldMobileCoin)

__NOTE__: The first release of wmcc-daemon.

---

**WorldMobileCoin** is a new cryptocurrency.

Official website: https://www.worldmobilecoin.com

## Installation Prerequisites
NodeJS (v8.0.0+) https://nodejs.org/en/  
GIT (v2) https://git-scm.com/downloads  
A proper C/C++ compiler:
> g++/gcc (Unix)  
> Microsoft Visual C++ Build Tools (Windows)  

** Please refer to [node-gyp](https://github.com/nodejs/node-gyp) for native build

To see example how to build on Ubuntu 16.04 from clean installation, click here [link](https://example.worldmobilecoin.com/ubuntu_16-04.html)

## Install
```
$ git clone git://github.com/worldmobilecoin/wmcc-daemon.git
$ cd wmcc-daemon
$ npm install
```

## Create Wallet
```
$ node ./bin/wallet

1) Enter 1
2) Enter Wallet Name
3) Enter Date of Birth
4) Enter Secret Question
5) Enter Secret Answer
6) Enter 1 to create wallet or 2 to add another secret

Done
```

## Get Passphrase
```
$ node ./bin/wallet

1) Enter 2
2) Enter Wallet Name
3) Enter Date of Birth
4) Enter Secret Answer

* Passphrase to be used in RPC/CLI.
```

## List of Wallets
```
$ node ./bin/wallet

1) Enter 3
```

## Run Node for the first time
```
$ node ./bin/node --wallet [walletname]
Eg: node ./bin/node --wallet "my wallet"

1) Wait for chain to synced
2) Or press cmd+c / ctrl+c
```

## Run Daemon
```
$ ./bin/wmccd --wallet [walletname]

* To make sure wmcc daemon is running, enter [IP]:7880 eg. http://127.0.0.1:7880 in your browser.
```

## API Documentation
https://docs.worldmobiecoin.com/api

## Disclaimer

WorldMobileCoin does not guarantee you against theft or lost funds due to bugs, mishaps,
or your own incompetence. You and you alone are responsible for securing your money.

## Contribution and License Agreement

If you contribute code to this project, you are implicitly allowing your code
to be distributed under the MIT license. You are also implicitly verifying that
all code is your original work.

## License

--Copyright (c) 2017, Park Alter (pseudonym)  
--Distributed under the MIT software license, see the accompanying  
--file COPYING or http://www.opensource.org/licenses/mit-license.php 