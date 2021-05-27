Pashto: `apertium-pus`
===============================================================================

This is an Apertium monolingual language package for Pashto. What
you can use this language package for:

* Morphological analysis of Pashto
* Morphological generation of Pashto
* Part-of-speech tagging of Pashto

Requirements
-------------------------------------------------------------------------------

You will need the following software installed:

* lttoolbox (>= 3.3.0)
* apertium (>= 3.3.0)
* vislcg3 (>= 0.9.9.10297)

If this does not make any sense, we recommend you look at: apertium.org.

Compiling
-------------------------------------------------------------------------------

Given the requirements being installed, you should be able to just run:

    $ ./configure
    $ make

You can use `./autogen.sh` instead of `./configure` if you're compiling
from source.

If you're doing development, you don't have to install the data, you
can use it directly from this directory.

If you are installing this language package as a prerequisite for an
Apertium translation pair, then do (typically as root / with sudo):

    # make install

You can give a `--prefix` to `./configure` to install as a non-root user,
but make sure to use the same prefix when installing the translation
pair and any other language packages.

Testing
-------------------------------------------------------------------------------

If you are in the source directory after running make, the following
commands should work:

    $  echo "TODO: test sentence" | apertium -d . pus-morph
    TODO: test analysis result

    $ echo "TODO: test sentence" | apertium -d . pus-tagger
    TODO: test tagger result

Files and data
-------------------------------------------------------------------------------

* `apertium-pus.pus.dix`            - Monolingual dictionary
* `pus.prob`                        - Tagger model
* `apertium-pus.pus.rlx`            - Constraint Grammar disambiguation rules
* `apertium-pus.post-pus.dix`       - Post-generator
* `modes.xml`                       - Translation modes

For more information
-------------------------------------------------------------------------------

* https://wiki.apertium.org/wiki/Installation
* https://wiki.apertium.org/wiki/apertium-pus
* https://wiki.apertium.org/wiki/Using_an_lttoolbox_dictionary

Help and support
-------------------------------------------------------------------------------

If you need help using this language pair or data, you can contact:

* Mailing list: apertium-stuff@lists.sourceforge.net
* IRC: `#apertium` on `irc.oftc.net`

See also the file AUTHORS included in this distribution.
