# Crypto

This repository contains implementations of some well-known ciphers.

## Getting Started
1.  Set up the python environment using conda:
    ```bash
    $ conda env create -f environment.yml
    ```
    or if you are not using conda, then make sure you have a python environment
    set up with all of the packages listed in the file `environment.yml`.
    
2.  Activate the conda environment:
    ```bash
    $ conda activate crypto
    ```
    
3.  Run a demo:
    ```bash
    $ python demos/caesar_cipher.py
    ```
    
    1.  Instead of typing out a message, you can pipe a text file into a demo 
        to use its contents as the message for the cipher to encrypt:
        ```bash
        $ python demos/caesar_cipher.py < sample_messages/helloworld.txt
        Enter a message to encrypt: 
        Message: HELLO WORLD
        ...
        ```
    
    2.  You can get the help text for each demo by adding the help option, e.g.:
        ```bash
        $ python demos/caesar_cipher.py --help
        ```
    
    3.  If you get an error such as:
        ```
        Traceback (most recent call last):
          File "demo/caesar_cipher.py", line 3, in <module>
            from ciphers.caesar import CaesarCipher
        ModuleNotFoundError: No module named 'ciphers'
        ```
        then add the current directory (should be the root directory of this repo) 
        to the python path as such:
        ```bash
        $ export PYTHONPATH=${PYTHONPATH}:${PWD}
        ```
