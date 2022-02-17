# Build Notes

## Installation 

### Ubuntu 20.04

Install nvidia-cuda-toolkit as root:
    
    # apt install nvidia-cuda-toolkit

Install nvm and node 10.24:

    $ curl -o- https://raw.githubusercontent.com/nvm-sh/nvm/v0.38.0/install.sh | bash
    $ nvm install lts/dubnium
    $ nvm use lts/dubnium

Install package dependencies from within the project directory by running

    $ npm install

Confirm that the app works by running and listing all accounts:

    $ node index.js

    command: account list

### Window 10

Download and install the NVIDIA Cuda Toolkit:

    https://developer.nvidia.com/cuda-downloads?target_os=Windows&target_arch=x86_64&target_version=10&target_type=exe_local

Install Python (v2 or 3):

    https://www.python.org/downloads/windows

Install Visual Studio (version 2019 or lower):

    https://visualstudio.microsoft.com/

Install Node.js v10.24.1 from:

    https://nodejs.org/dist/latest-dubnium/node-v10.24.1-x64.msi

Alternatively, install Node Version Manager for Windows:

    https://github.com/coreybutler/nvm-windows

and, from the administrator command prompt, run 

    > nvm install lts/dubnium
    > nvm use lts/dubnium

Open a new command prompt and navigate to the source location. Run

    > npm install

to install project dependencies.  

Finally, confirm that the app works by running and listing all accounts:

    > node index.js

    command: account list


## Bundling a standalone executable 

Package into a standalone executable by running:

    npm run package

Test the executable by moving it to another location and running

    cosmic-v3.4t

from the location you've moved it to.
