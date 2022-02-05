# Build Notes

## Installation 

Install nvidia-cuda-toolkit on Ubuntu 20.04 as root
    
    # apt install nvidia-cuda-toolkit

Or on Windows 10, download and install from

    https://developer.nvidia.com/cuda-downloads?target_os=Windows&target_arch=x86_64&target_version=10&target_type=exe_local

Install nvm and node 10.24 on Ubuntu 20.04:

    $ curl -o- https://raw.githubusercontent.com/nvm-sh/nvm/v0.38.0/install.sh | bash
    $ nvm install lts/dubnium
    $ nvm use lts/dubnium

On Windows 10, it is recommended to install Node.js directly from

    https://nodejs.org/dist/latest-dubnium/node-v10.24.1-x64.msi

Install package dependencies from with the project directory by running

    $ npm install

Confirm that the app works by running and listing all accounts:

    $ node index.js

    command: account list


## Bundling a standalone executable 

Package into a standalone executable by running:

    $ npm run package

Test the executable by moving it to another location and running

    $ ./cosmic-v3.4t

from the location you've moved it to.
