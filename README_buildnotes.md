# Build Notes

## Installation on Ubuntu 20.04

Install nvm 

    $ curl -o- https://raw.githubusercontent.com/nvm-sh/nvm/v0.38.0/install.sh | bash

Install node 10.24 by running

    $ nvm install lts/dubnium
    $ nvm use lts/dubnium


Install yarn and node-gyp

    $ npm install -g yarn node-gyp

Run yarn from within the top level of the source directory to install dependencies.

    $ yarn 

Confirm that the app works by running and listing all accounts:

    $ node index.js

    command: account list

## Bundling a standalone executable

Navigate to the source directory and add the local node modules to the path:

    $ export PATH=`pwd`/node_modules/.bin:$PATH

Package into a standalone executable for linux by running:

    $ pkg -o 0xbitcoin-gpuminer -t node10-linux-x64 index.js

