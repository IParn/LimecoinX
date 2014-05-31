LimeCoin X11 cryptoCurrency
================================





<img src="http://209.208.111.8/splash.png" alt="Limecoin">

http://www.LimeCoin.org


Copyright (c) 2009-2014 Bitcoin Developers
Copyright (c) 2013-2014 limecoin Developers

What is LimeCoinX?
----------------

LimeCoinX is the Second Generation of LimeCoin a cryptocurrency based in DarkCoin using X11 as a proof-of-work algorithm.
 - Super secure hashing algorithm: 11 rounds of scientific hashing functions (blake, bmw, groestl, jh, keccak, skein, luffa, cubehash, shavite, simd, echo)
 - GPU/CPU only mining
 - Block generation: 5 minutes
 - Difficulty Retargets every 18 block using Dark Gravity Wave 3
 - Est. ~5,2M Coins in 2015, ~10,4M in 2016.
 - Anonymous blockchain using DarkSend technology (August 2014)
 - Block Reward: 50 Coins
 - Premine: 2% 

For more information, as well as an immediately useable, binary version of
the LimeCoin client sofware, see http://www.LimeCoin.org



Benefits of Using LimeCoinX
--------------------------

X11 - Originally from Darkcoin and created by Evan Duffield. X11 uses the following for complex hashing:
blake, bmw, groestl, jh, keccak, skein, luffa, cubehash, shavite, simd and echo. 

Energy Saving - Since X11 is much less strenuous on graphics cards, it runs a lot cooler and saves a lot on electricity costs. 
This is an extremely important factor, the X11 algo can run coolly without any added external cooling and hence allowing 
for more underclocking and undervolting. It�s a win-win situation!

There is GPU mining software available for X11 which makes it a suitable hashing solution.

QR Code - LimeCoin has built in QR code support so you can generate QR codes from within the software.

DNS Seed Node - This is used by nodes to find others on the network meaning that when you turn
Limecoin on it connects to he DNS Seed node to find other Limecoin clients without any manual effort.





License
-------

limecoin is released under the terms of the MIT license. See `COPYING` for more
information or see http://opensource.org/licenses/MIT.

Development process
-------------------

Developers work in their own trees, then submit pull requests when they think
their feature or bug fix is ready.

If it is a simple/trivial/non-controversial change, then one of the limecoin
development team members simply pulls it.

If it is a *more complicated or potentially controversial* change, then the patch
submitter will be asked to start a discussion (if they haven't already) on the
[mailing list](http://sourceforge.net/mailarchive/forum.php?forum_name=bitcoin-development).

The patch will be accepted if there is broad consensus that it is a good thing.
Developers should expect to rework and resubmit patches if the code doesn't
match the project's coding conventions (see `doc/coding.txt`) or are
controversial.

The `master` branch is regularly built and tested, but is not guaranteed to be
completely stable. [Tags](https://github.com/bitcoin/bitcoin/tags) are created
regularly to indicate new official, stable release versions of limecoin.

Testing
-------

Testing and code review is the bottleneck for development; we get more pull
requests than we can review and test. Please be patient and help out, and
remember this is a security-critical project where any mistake might cost people
lots of money.

### Automated Testing

Developers are strongly encouraged to write unit tests for new code, and to
submit new unit tests for old code.

Unit tests for the core code are in `src/test/`. To compile and run them:

    cd src; make -f makefile.unix test

Unit tests for the GUI code are in `src/qt/test/`. To compile and run them:

    qmake BITCOIN_QT_TEST=1 -o Makefile.test bitcoin-qt.pro
    make -f Makefile.test
    ./limecoin-qt_test

LimeCoin Updated Windows Wallet Compiling guide
-------------------------------

Click on Windows Logo:

<a href="https://github.com/IParn/limecoin/blob/master/contrib/gitian-descriptors/README.md"><img src="http://www.avirecomp.com/e107_files/images/screenshots/Vista_logo_small.png" alt="Windows Wallet"></a></p>


