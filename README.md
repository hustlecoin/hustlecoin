Hustlecoin Core integration/staging tree
========================================

http://hustlecoin.today/

What is Hustlecoin?
-------------------

Hustlecoin is an experimental digital currency that enables instant payments to
anyone, anywhere in the world. Hustlecoin uses peer-to-peer technology to operate
with no central authority: managing transactions and issuing money are carried
out collectively by the network. Hustlecoin Core is the name of open source
software which enables the use of this currency.

License
-------

Hustlecoin Core is released under the terms of the MIT license. See [COPYING](COPYING) for more
information or see https://opensource.org/licenses/MIT.

How to build
------------

```
git clone https://github.com/hustlecoin/hustlecoin
cd hustlecoin/depends
make HOST=x86_64-linux-gnu -j4
cd ..
./autogen.sh
CONFIG_SITE=$PWD/depends/x86_64-linux-gnu/share/config.site ./configure
make -j4
```

replacing x86_64-linux-gnu with the appropriate platform to crosscompile for

How to stratum
--------------

As usual:

Just remember 0.21 base does not create a wallet automatically. Issue 'createwallet ""'
to create one.
