SublimeIPython
==============
An [IPython](http://ipython.org/) plugin for [Sublime Text](http://www.sublimetext.com/)

**Note:** this project was originally created by @bonsoir.

Features
--------

* Running code in IPython
* Auto completion with IPython

Installation
------------

1. Find your Sublime Text Packages directory

   On your Sublime Text menu, choose **Preferences | Browse Packages...**, the Packages directory should display.

2. Install plugin code

   If you have git, clone SublimeIPython to Sublime Text Packages directory:

        git clone git@github.com:iambus/SublimeIPython.git

   If you don't have git, click [here](https://github.com/iambus/SublimeIPython/archive/master.zip) to download a latest zipball, unzip it to Sublime Text Packages (rename unzipped folder to SublimeIPython).

   Make sure the directory structure is correct:

        Packages
        └─SublimeIPython
            │  SublimeIPython.py
            │  ipython_output.tmLanguage
            └─sublime_ipython

3. Install dependencies

   **On Windows**, download [x86](https://github.com/downloads/iambus/SublimeIPython/SublimeIPython-depends-win32-x86-nightly.zip) or [x64](https://github.com/downloads/iambus/SublimeIPython/SublimeIPython-depends-win64-x64-nightly.zip) dependency file. Unzip it to Packages/SublimeIPython.

      **Note:** you should use x64 dependency file if and only if you are using 64-bit Sublime Text, e.g. **Sublime Text 2.0.1 x64 Setup.exe** or **Sublime Text 2.0.1 x64.zip**.

      Make sure the directory structure is correct:

         Packages
         └─SublimeIPython
             │  SublimeIPython.py
             │  ipython_output.tmLanguage
             │  path.py
             ├─sublime_ipython
             ├─IPython
             ├─zmq
             ├─sqlite3
             └─distutils

   **On Linux**, I will try it later...

4. Launch IPython

   Install [IPython](http://ipython.org/), and launch an IPython instance:

        ipython console

5. Key bindings

   On your Sublime Text menu, choose **Preferences | Key bindings - User**, input the key bindings and save the changes:

        [
        	{ "keys": ["ctrl+enter"], "command": "ipython_exec" },
        	{ "keys": ["f5"], "command": "ipython_exec_file" }
        ]

   If your already have some user key bindings, merge the list yourself.

5. A final test

   Now the installation is complete. Restart your Sublime Text, create a Python file and write some code. You can use **ctrl+enter** to execute current line, **f5** to execute the whole file.

Troubleshooting
---------------

If it doesn't work, press **ctrl+`** and check if there is any error in the console.

License
-------

Copyright (C) 2012

Distributed under the MIT License.

