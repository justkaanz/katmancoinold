Katmancoin integration/staging tree
================================

http://www.katmancoin.org

Copyright (c) 2009-2014 Bitcoin Developers

Copyright (c) 2011-2014 Litecoin Developers

Copyright (c) 2021 Katmancoin Developer

What is Katmancoin?
----------------

Katmancoin is a lite version of Bitcoin using scrypt as a proof-of-work algorithm.
 - 5 minute block targets
 - subsidy halves in 1,26 million blocks (~6 years)
 - ~126 million total coins

The rest is the same as Bitcoin.
 - 20 coins per block

It is an altcoin created for entertainment and humor purposes.

For more information, as well as an immediately useable, binary version of
the Katmancoin client sofware, see http://www.katmancoin.org.(not yet)


What is Katman?
---------------
The formation founded by Çağrı Ergün, where his audience gathered.
There are no illegal or defamatory elements on this page, this is a piece of humor from the discord community called KATMAN. Over and over; Responsibility belongs to our MNT license.
twitch.tv/HYPE discord.gg/HYPE


What is Nuribet?
---------------
Nuribet is a Turkish online prediction company holding the Curaçao eGaming License. It was established in 2020 and registered in Cyprus. In 2019, they experienced significant growth by sponsoring Chelsea FC, Liverpool FC and Tottenham Hotspur briefly. He is currently continuing on Twitch on the HYPE channel on our new chip system, the prediction system.
You can visit our site for 30% Loss bonus, 50 offspins and more.

https://youtu.be/rxkkD3_A9jM
Today they are playing with katmancoin at low risk.


License
-------

Katmancoin is released under the terms of the MIT license. See `COPYING` for more
information or see http://opensource.org/licenses/MIT.
+
Our second license is reserved under Batuhamnt's hair. If you want to 
see and get information https://twitch.tv/batuhanmnt

Development process
-------------------

Developers work in their own trees, then submit pull requests when they think
their feature or bug fix is ready.

If it is a simple/trivial/non-controversial change, then one of the Katmancoin
development team members simply pulls it.

If it is a *more complicated or potentially controversial* change, then the patch
submitter will be asked to start a discussion with the devs and community.

The patch will be accepted if there is broad consensus that it is a good thing.
Developers should expect to rework and resubmit patches if the code doesn't
match the project's coding conventions (see `doc/coding.txt`) or are
controversial.

The `master` branch is regularly built and tested, but is not guaranteed to be
completely stable. [Tags](https://github.com/katmancoin-project/katmancoin/tags) are created
regularly to indicate new official, stable release versions of Katmancoin.

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
    ./katmancoin-qt_test

