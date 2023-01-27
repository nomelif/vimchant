Vimchant
========

**Enchant-based on-the-fly spell-checker for Vim text editor**

*Note:* This program is not maintained. You are free to adopt it,
maintain and develop it further.

Vim 7.0 introduced excellent spell-checking features which made external
spell-checker plugins pretty much obsolete. Unfortunately not all
languages can be supported through Vim’s dictionary format. Either the
language is morphologically too complex or better custom solutions exist
already for some languages—solutions which are not compatible with Vim’s
spelling checker. Finnish, for example, is a language which doesn’t
currently benefit from Vim’s spell-checking features.

This plugin (Vimchant) provides a simple but fast on-the-fly spelling
checker which uses [Enchant][] as its back-end program. Enchant is a
spell-checker library and utility included in modern GNU/Linux systems.
Enchant itself is only a front-end for many different spell-checkers,
including Voikko, Zemberek, Hunspell, Hspell, Uspell, Myspell, Aspell
and Ispell. All the spell-checkers and languages which can be supported
through Enchant are available to Vim through this plugin.

Manual for Vimchant is included, just type:

    :help vimchant.txt


Usage
-----

The most interesting commands are `\ss` (spell-checker on/off) and `\sl`
(change language). The default interval period before running the
spell-check is rather long (4 seconds). To make the spell-checker
respond faster (1 second, for example) add the following line to your
Vim configuration file:

    set updatetime=1000

See the included Vim manual for more info.


Author and License
------------------

Author: Teemu Likonen <<tlikonen@iki.fi>>

OpenPGP key: [6965F03973F0D4CA22B9410F0F2CAE0E07608462][PGP]

License: [Creative Commons CC0][CC0] (public domain dedication)


[Enchant]: https://abiword.github.io/enchant/
[PGP]:     http://www.iki.fi/tlikonen/pgp-key.asc
[CC0]:     https://creativecommons.org/publicdomain/zero/1.0/legalcode
