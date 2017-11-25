Dimecoin 1.6.9 BETA
====================

Copyright (c) 2009-2013 Bitcoin Developers
Copyright (c) 2013-2014 Dimecoin Developers

Distributed under the MIT/X11 software license, see the accompanying
file COPYING or http://www.opensource.org/licenses/mit-license.php.
This product includes software developed by the OpenSSL Project for use in the [OpenSSL Toolkit](http://www.openssl.org/). This product includes
cryptographic software written by Eric Young ([eay@cryptsoft.com](mailto:eay@cryptsoft.com)), UPnP software written by Thomas Bernard and
sphlib 3.0 by Thomas Pornin.


Intro
---------------------
Dimecoin is a free open source peer-to-peer electronic cash system that is
completely decentralized, without the need for a central server or trusted
parties.  Users hold the crypto keys to their own money and transact directly
with each other, with the help of a P2P network to check for double-spending.


Setup
---------------------

Compiling and configuring Dimecoin-Qt from source on Ubuntu.

https://www.youtube.com/watch?v=yW1-kSrQM10

(
if during compiling you get an error:
alert.cpp:268:1: fatal error: opening dependency file obj/alert.d:
No such file or directory compilation terminated.
make: *** [obj/alert.o] Error 1

please use command:

mkdir obj

and next:

make -f makefile.unix "USE_UPNP=-"

if you get later second error:
g++: /coins7ex/dimecoin/src/leveldb/libmemenv.a: No such file or
directory
make: *** [dimecoind] Error 1

please open leveldb and use command:

make libleveldb.a libmemenv.a

and go back to compiling.
)
