Installation Procedures
=======================

#Install and setting up virtualenv.
    Documentation: https://virtualenv.pypa.io/en/latest/
    Github: https://github.com/pypa/virtualenv

    ###Installation
    Using pip to install: pip install virtualenv
    Install from source:
        ```chef
        $ git clone https://github.com/pypa/virtualenv
        $ cd virtualenv
        $ [sudo] python setup.py install
        ```
    ###Setting up new virtual environment
        ```chef
        $ virtualenv nodejs --no-site-packages
        ```
    ###Using the virtual environment
        ```chef
        $ cd nodejs
        $ source bin/activate
        ```

#Download, compile and install the latest nodejs
    Documentation: http://nodejs.org/documentation/
    Github: https://github.com/joyent/node

    ```chef
    $ curl http://nodejs.org/dist/node-latest.tar.gz | tar xvz
    $ cd node-v0.10.36
    $ ./configure --prefix=$VIRTUAL_ENV
    $ make install
    ```
