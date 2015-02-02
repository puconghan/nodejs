Installation Procedures
=======================

#Install and set up virtualenv.
    Documentation: https://virtualenv.pypa.io/en/latest/
    Github: https://github.com/pypa/virtualenv

    ###Installation
    Using pip to install: pip install virtualenv
    Install from source:
        $ git clone https://github.com/pypa/virtualenv
        $ cd virtualenv
        $ [sudo] python setup.py install
    ###Setting up new virtual environment
        $ virtualenv nodejs --no-site-packages
    ###Using the virtual environment
        $ cd nodejs
        $ source bin/activate

#Compile and install the latest nodejs
    Documentation: http://nodejs.org/documentation/
    Github: https://github.com/joyent/node

    Prerequisites (Unix only):
        * GCC 4.2 or newer
        * G++ 4.2 or newer
        * Python 2.6 or 2.7
        * GNU Make 3.81 or newer
        * libexecinfo (FreeBSD and OpenBSD only)

    $ curl http://nodejs.org/dist/node-latest.tar.gz | tar xvz
    $ cd node-v0.10.36
    $ ./configure --prefix=$VIRTUAL_ENV
    $ make install
