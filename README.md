# BASE64-Encoder-Decoder
creating a tool to encode and decode text using BASE64, a common data encoding method in cybersecurity


It aims to provide a fast base64 implementation for base64 encoding/decoding.

Installation
pip install pybase64
Usage
pybase64 uses the same API as Python base64 "modern interface" (introduced in Python 2.4) for an easy integration.

To get the fastest decoding, it is recommended to use the pybase64.b64decode and validate=True when possible.

import pybase64

print(pybase64.b64encode(b'>>>foo???', altchars='_:'))
# b'Pj4_Zm9vPz8:'
print(pybase64.b64decode(b'Pj4_Zm9vPz8:', altchars='_:', validate=True))
# b'>>>foo???'

# Standard encoding helpers
print(pybase64.standard_b64encode(b'>>>foo???'))
# b'Pj4+Zm9vPz8/'
print(pybase64.standard_b64decode(b'Pj4+Zm9vPz8/'))
# b'>>>foo???'

# URL safe encoding helpers
print(pybase64.urlsafe_b64encode(b'>>>foo???'))
# b'Pj4-Zm9vPz8_'
print(pybase64.urlsafe_b64decode(b'Pj4-Zm9vPz8_'))
# b'>>>foo???'
A command-line tool is also provided. It has encode, decode and benchmark subcommands.

usage: pybase64 [-h] [-V] {benchmark,encode,decode} ...

pybase64 command-line tool.

positional arguments:
  {benchmark,encode,decode}
                        tool help
    benchmark           -h for usage
    encode              -h for usage
    decode              -h for usage

optional arguments:
  -h, --help            show this help message and exit
  -V, --version         show program's version number and exit
Full documentation on : http://pybase64.readthedocs.io/en/stable/?badge=stable
