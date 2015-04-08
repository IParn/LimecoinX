*This is a draft!*

0.11.2 Release notes
====================


Limecoinx Core version 0.11.2 is now available from:

  https://limx.eu

Please report bugs using the issue tracker at github:

  https://github.com/LIMX-SUPPORT/LimecoinX


Mining and relay policy enhancements
------------------------------------

Limecoinx Core's block templates are now for version 3 blocks only, and any
mining software relying on its `getblocktemplate` must be updated in parallel
to use libblkmaker either version 0.4.2 or any version from 0.5.1 onward. If you
are solo mining, this will affect you the moment you upgrade Limecoinx Core,
which must be done prior to BIP66 achieving its 951/1001 status. If you are
mining with the stratum mining protocol: this does not affect you. If you are
mining with the getblocktemplate protocol to a pool: this will affect you at the
pool operator's discretion, which must be no later than BIP66 achieving its
951/1001 status.


BIP 66: strict DER encoding for signatures
------------------------------------------

Limecoinx Core 0.11.2 implements BIP 66, which introduces block version 3, and a
new consensus rule, which prohibits non-DER signatures. Such transactions have
been non-standard since Limecoinx 0.8, but were technically still permitted
inside blocks.

This change breaks the dependency on OpenSSL's signature parsing, and is
required if implementations would want to remove all of OpenSSL from the
consensus code.

The same miner-voting mechanism as in BIP 34 is used: when 751 out of a
sequence of 1001 blocks have version number 3 or higher, the new consensus
rule becomes active for those blocks. When 951 out of a sequence of 1001
blocks have version number 3 or higher, it becomes mandatory for all blocks.

Backward compatibility with current mining software is NOT provided, thus
miners should read the first paragraph of "Mining and relay policy
enhancements" above.

Also compare with [upstream release notes](https://github.com/bitcoin/bitcoin/blob/0.10/doc/release-notes.md#mining-and-relay-policy-enhancements).

More info on [BIP 66](https://github.com/bitcoin/bips/blob/master/bip-0066.mediawiki).


How to Upgrade
--------------

If you are running an older version, shut it down. Wait until it has completely
shut down (which might take a few minutes for older versions), then run the
installer (on Windows) or just copy over /Applications/Limecoinx-Qt (on Mac) or
limecoinxd/limecoinx-qt (on Linux).


0.11.2 changelog
----------------

- *to do ..*


Credits
--------

Thanks to who contributed to this release, at least:

- *to do ..*

As well as everyone that helped translating on [Transifex](https://www.transifex.com/projects/p/limecoinx/).
